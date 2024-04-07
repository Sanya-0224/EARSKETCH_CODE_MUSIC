# description: 
#Script_name: Music

#author: Learning with coursera
#description: composition practice

#SET UP
from earsketch import *

init()
setTempo(120) #ypically means setting the tempo of a piece of music to 120 beats per minute (BPM). 
# Music
#fetch from API list
#fitMedia is a shell that requires 4 parameter (sound,track,start and end)start location is beginning measure and the end is attending leisureRD_UK_HOUSE__5THCHORD_2 
fitMedia(RD_UK_HOUSE__5THCHORD_2, 1, 1, 16)#1 track no 1 start measure and 16 end measure
#  ADD EFFECT BETWEEN MEASURES 1 AND 16 MOVING FROM -60DB TO 50DB AND BACK DOWN
setEffect(1, VOLUME, GAIN, -60, 1 , 5, 12)
setEffect(1, VOLUME, GAIN, 5, 12, -60, 16)
fitMedia(HIPHOP_DUSTYGUITAR_001, 2, 1, 12)
#  ADD EFFECTS
setEffect(2, DELAY, DELAY_TIME, 500)
fitMedia(HOUSE_MAIN_BEAT_003, 3 , 1 , 8)
#  ADD EFFECT
setEffect(3, REVERB, REVERB_TIME, 200)
finish()#tells that our code is finish and ready to run
