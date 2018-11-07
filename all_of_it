
x = c(2,3,7,2,6)
y = c(10,8,7,5,10)
z = c(10,13,14,13,15)
w = c(x,y,z)

ssw <- ((length(x)-1)*(sd(x)^2) + (length(y)-1)*(sd(y)^2) + (length(z)-1)*(sd(z)^2))

ssb <- length(x)*((mean(x)-mean(w))^2) +  length(y)*((mean(y)-mean(w))^2) + length(z)*((mean(z)-mean(w))^2)

sst <- ssw + ssb

dfb <- 3-1
#3 is the number of groups
dfw <- length(w) - 3
#number of samples in all groups minus number of groups

ssbdf <- ssb/dfb
sswdf <- ssw/dfw

f <- ssbdf/sswdf
qf(.95, dfb, dfw)

#if qf is less than f, then you reject null

sd(w)
sqrt(((sd(x)^2)*(3) + (sd(y)^2)*(3) + (sd(z)^2)*(3))/9)
