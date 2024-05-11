# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Fitting Generalized Nonlinear Models Use gnm With (In) R Software
install.packages("gnm")
library("gnm")
# Import Data Excel Into R From Github Olah Data Semarang (timbulwidodostp)
gnm = read.csv("https://github.com/timbulwidodostp/gnm/raw/main/gnm/gnm.csv",sep = ";")
# Estimate Fitting Generalized Nonlinear Models Use gnm With (In) R Software
gnm<-gnm(Freq~election:vote+election:class:religion+Mult(Exp(election),religion:vote)+Mult(Exp(election),class:vote),family=poisson,data=gnm)
summary(gnm)
# Fitting Generalized Nonlinear Models Use gnm With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished
