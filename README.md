# NoahBMicroBit

#Who
  #Noah Baumann
  #Linsey
#What
  #this creates a wave on the microbit which cycles. first the first column lights up, then the first and second, Etc.  
  
#How
  #I created 5 images, then made a list out of each of the all five images. then I cycle through the list and display each image in order. 


#Why

I thought it would look cool, and I am not dissapointed. 


#code:
 # Add your Python code here. E.g.
from microbit import *

wave1 = Image("00000000000000000000")
wave2 = Image("90000:90000:90000:90000:90000")
wave3 = Image("99000:99000:99000:99000:99000")
wave4 = Image("99900:99900:99900:99900:99900")
wave5 = Image("99990:99990:99990:99990:99990")
wave = [wave1, wave2, wave3, wave4, wave5, wave5, wave4, wave3, wave2, wave1]
while True:
    display.show(wave, loop = True, delay = 100)
    display.show(Image.HEART)
    sleep(2000)
