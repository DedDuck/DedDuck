def intro():
    while ((v*t)<b/2):
        r = (v * t)
        s = r**2*pi
        print('Площадь пожара равна: ', s, end='\n\n')
        break
    while (((v * t)>b/2) and ((v * t)<a)):
        s = b*(v * t)
        print('Площадь пожара равна: ', s, end='\n\n')
        break
    if ((v * t)>a):
        print('Горит все помещение, Площадь пожара равна: ',a*b)

print('Для выхода введите "стоп".')

a = 52
b = 26
pi = 3.14
good = 'да'
while good != 'стоп':
    v1 = input('Введите скорость распространения пожара: ')
    v = float(v1)
    t1 = input('Введите сколько прошло времени с начала пожара: ')
    t = float(t1)
    intro()
    good = input('Удовлетворяют данные? ')
