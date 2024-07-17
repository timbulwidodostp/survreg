# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Regression for a Parametric Survival Model Use survreg With (In) R Software
install.packages("survival")
library("survival")
survreg = read.csv("https://raw.githubusercontent.com/timbulwidodostp/survreg/main/survreg/survreg.csv",sep = ";")
# Estimation Regression for a Parametric Survival Model Use survreg With (In) R Software
survreg_weibull <- survreg(Surv(futime, fustat) ~ ecog.ps + rx, survreg, dist='weibull', scale=1)
summary(survreg_weibull)
survreg_exponential <- survreg(Surv(futime, fustat) ~ ecog.ps + rx, survreg, dist="exponential")
summary(survreg_exponential)
# Regression for a Parametric Survival Model Use survreg With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished