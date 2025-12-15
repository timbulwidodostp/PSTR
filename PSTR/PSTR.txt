# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Panel Smooth Transition Regression (PSTR) model Use NewPSTR And EstPSTR (PSTR) With (In) R Software
install.packages("remotes")
remotes::install_github("yukai-yang/PSTR")
library("PSTR")
library("tibble")
# Estimation Panel Smooth Transition Regression (PSTR) model Use NewPSTR And EstPSTR (PSTR) With (In) R Software
PSTR = read.csv("https://raw.githubusercontent.com/timbulwidodostp/PSTR/main/PSTR/PSTR.csv",sep = ";")
PSTR <- as_tibble(PSTR)
PSTR = NewPSTR(PSTR, dep = 'inva', indep = 4:20, indep_k = c('vala','debta','cfa','sales'), tvars = c('vala'), im = 1, iT = 14)
PSTR
PSTR = EstPSTR(use = PSTR)
PSTR
# Panel Smooth Transition Regression (PSTR) model Use NewPSTR And EstPSTR (PSTR) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished