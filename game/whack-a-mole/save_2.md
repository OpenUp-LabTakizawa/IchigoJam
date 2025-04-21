10 CLS:PRINT "GAME OVER       "
20 gosub 300
30 PLAY "O4T180"
40 IF S<25 GOTO 90
50 LC 0,1:PRINT "ｵﾐｺﾞﾄ!!         ":gosub 300
60 gosub 370:wait60:gosub 360:wait60:gosub 340:wait60:LED1:IF BTN()=0 GOTO 60
70 PLAY ">C<BAG>C<BAG>CED"
80 GOTO 190
90 IF S<20 GOTO 130
100 LC 0,1:PRINT "ﾅｶﾅｶ ﾔﾙﾅ!       ":gosub 300:gosub 330
110 PLAY "CEG>C"
120 GOTO 190
130 IF S<10 GOTO 170
140 LC 0,1:PRINT "ﾏｱﾏｱ ｶﾅ?        ":gosub 300:gosub 350
150 PLAY "AF"
160 GOTO 190
170 LC 0,1:PRINT "ｳｰﾑ ｻﾞﾝﾈﾝ       ":gosub 300:gosub 370
180 PLAY "A"
190 LED1:IF BTN()=0 GOTO 190
200 LED0:LRUN 00
300 wait10
310 ifi2cw(62,#701,1,#702,1)+i2cw(62,#700,1,#900,16)+i2cw(62,#701,1,#703,1)+i2cw(62,#700,1,#920,16)?"E"
320 return
330 ifi2cw(98,#711,1,#715,1)+i2cw(98,#712,1,#715,1)+i2cw(98,#713,1,#714,1)?"E"
340 return
350 ifi2cw(98,#711,1,#715,1)+i2cw(98,#712,1,#714,1)+i2cw(98,#713,1,#715,1)?"E"
360 return
370 ifi2cw(98,#711,1,#714,1)+i2cw(98,#712,1,#715,1)+i2cw(98,#713,1,#715,1)?"E"
380 return
