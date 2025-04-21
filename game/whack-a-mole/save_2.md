220 CLS:PRINT "GAME OVER       "
230 gosub 900
240 PLAY "O4T180"
250 IF S<25 GOTO 290
260 LC 0,1:PRINT "ｵﾐｺﾞﾄ!!         ":gosub 900
265 gosub 970:wait60:gosub 960:wait60:gosub 940:wait60:LED1:IF BTN()=0 GOTO 265
270 PLAY ">C<BAG>C<BAG>CED"
280 GOTO 390
290 IF S<20 GOTO 330
300 LC 0,1:PRINT "ﾅｶﾅｶ ﾔﾙﾅ!       ":gosub 900:gosub 940
310 PLAY "CEG>C"
320 GOTO 390
330 IF S<10 GOTO 370
340 LC 0,1:PRINT "ﾏｱﾏｱ ｶﾅ?        ":gosub 900:gosub 960
350 PLAY "AF"
360 GOTO 390
370 LC 0,1:PRINT "ｳｰﾑ ｻﾞﾝﾈﾝ       ":gosub 900:gosub 970
380 PLAY "A"
390 LED1:IF BTN()=0 GOTO 390
400 LED0:LRUN 00
900 wait10
910 ifi2cw(62,#701,1,#702,1)+i2cw(62,#700,1,#900,16)+i2cw(62,#701,1,#703,1)+i2cw(62,#700,1,#920,16)?"E"
920 return
925
930
940 ifi2cw(98,#711,1,#715,1)+i2cw(98,#712,1,#715,1)+i2cw(98,#713,1,#714,1)?"E"
945 return
960 ifi2cw(98,#711,1,#715,1)+i2cw(98,#712,1,#714,1)+i2cw(98,#713,1,#715,1)?"E"
965 return
970 ifi2cw(98,#711,1,#714,1)+i2cw(98,#712,1,#715,1)+i2cw(98,#713,1,#715,1)?"E"
975 return
