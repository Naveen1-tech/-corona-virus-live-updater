# -n CodePython
from bs4 import BeautifulSoup as bf
import requests
import time
from boltiot import Bolt
import ssl
a = list()
#———————-Algorithum  to compare the values every 10 min—————





def checking1(x,count):
  a.insert(count,x)
  if count == 1:
    print(a)
    if(a[1]-a[0] > 10):
      a.clear()
      return(1)
    else:
      a.clear()
      return(0)
