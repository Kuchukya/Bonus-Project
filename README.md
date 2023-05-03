# Bonus_Project 
import time
import datetime


def countdown(h, m, s):
  my_seconds = h * 3600 + m * 60 + s
  while my_seconds > 0:
    timer = datetime.timedelta(seconds=my_seconds)
    print(str(timer))
    time.sleep(1)
    my_seconds -= 1
  print("The countdown has finished!!")


time_str = input("Enter the time in the format 'h:m:s': ")
h, m, s = map(int, time_str.split(':'))
countdown(h, m, s)
