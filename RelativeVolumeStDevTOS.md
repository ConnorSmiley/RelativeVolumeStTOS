#defining variable of RelativeVolumeStDev(*Days) with StandardDev of *3\
def volumeCondition = RelativeVolumeStDev(50).RelVol >= 3;\
#scan if volumneCondition is over 3 for 5 days\
plot signal = Sum(volumeCondition, 5) >= 3;