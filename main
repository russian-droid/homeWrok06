#Write a function fuzzy_time which expects a time string
#in the form hh: mm (e.g. "12:25", "04:56"). The function
#rounds up or down to a quarter of an hour. Examples:
#fuzzy_time("12:58") ---> "13

def fuzzy_time(hrs, min):
    if min == 0:
        min = ':00'
    elif 0 < min <= 15:
        min = ':15'
    elif min <= 30:
        min = ':30'
    elif min <= 45:
        min = ':45'
    elif min > 45:
        min = ':00'
        h = int(hrs) + 1
        hrs = str(h)
    else:
        pass
    #
    print('Rounded time: ',hrs,min)

hrs=int(input("Input hrs >>> "))
min=int(input("Input min >>> "))

fuzzy_time(hrs,min)

#------------------------------------------
#a try with actual time
#  
from datetime import datetime, timedelta

def fuzzy_time(dt, delta):
    return dt + (datetime.min - dt) % delta

now = datetime.now()
print('actual time >>> ', now)
print('rounded time >>> ', fuzzy_time(now, timedelta(minutes=15))) #enter rounding minutes
