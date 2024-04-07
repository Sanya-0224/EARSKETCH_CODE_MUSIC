#description: composition practice

#SET UP
from earsketch import *

init()
setTempo(120) #ypically means setting the tempo of a piece of music to 120 beats per minute (BPM). 
# Music

#fetch from API list
#fitMedia is a shell that requires 4 parameter (sound,track,start and end)start location is beginning measure and the end is attending leisureRD_UK_HOUSE__5THCHORD_2 
fitMedia(SANYA_UPPAL_JAB_TAK_HE_JAAN, 1, 1, 11)
fitMedia(SANYA_UPPAL_MAIN_YAHAA_HOO, 1, 11, 15)
setEffect(1, VOLUME, GAIN, -18, 1, 5, 12)
setEffect(1, VOLUME, GAIN, 5, 2, -10, 16)
fitMedia(SANYA_UPPAL_MAIN_YAHAA_HOO, 1, 4, 9)
fitMedia(SANYA_UPPAL_BHOLI_SI_SURAT, 2, 3, 10)#1 track no 1 start measure and 16 end measure
#  ADD EFFECT BETWEEN MEASURES 1 AND 16 MOVING FROM -60DB TO 50DB AND BACK DOWN
setEffect(1, VOLUME, GAIN, -60, 1, 5, 12)
setEffect(1, VOLUME, GAIN, 5, 2, -50, 16)
fitMedia(SANYA_UPPAL_RABNEB_54B685C74639738, 3, 6, 10)
fitMedia(SANYA_UPPAL_AWESOME_WHISTLE, 4, 14, 17)
setEffect(2, REVERB, REVERB_TIME, 200)

#  ADD EFFECTS
setEffect(2, VOLUME, GAIN, -18, 3, 5, 12)
setEffect(2, VOLUME, GAIN, 2, 3, 10, 16)
setEffect(2, REVERB, REVERB_TIME, 200)


finish()#tells that our code is finish and ready to run
