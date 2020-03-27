[Think Stats Chapter 5 Exercise 1](http://greenteapress.com/thinkstats2/html/thinkstats2006.html#toc50) (blue men)

#convert feet and inches into cm

def convertToCM(feet, inch):

    cm = 30.5*feet+2.5*inch
    
    return cm
 
blueman_min = convertToCM(5, 10)
 
blueman_min = convertToCM(6, 1)

import scipy.stats

bman_low=scipy.stats.norm.cdf(blueman_min, loc= 178, scale=7.7 )

bman_high=scipy.stats.norm.cdf(blueman_max, loc= 178, scale=7.7 )

bman_high-bman_low

0.36086532777380054

# So there are 36% of male who are eligible for Blue Man Group
