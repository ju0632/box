
=IFS(OR(SUBSTITUTE($A1,"  ","")="{",SUBSTITUTE($A1,"  ","")="},",SUBSTITUTE(RIGHT($A1,1),"  ","")="[",SUBSTITUTE($A1,"  ","")="],"),1)

=IFS(OR(SUBSTITUTE(RIGHT($A1,1),"  ","")="[",SUBSTITUTE($A1,"  ","")="],"),1)

=IFS(OR(SUBSTITUTE($A1,"  ","")="{",SUBSTITUTE($A1,"  ","")="},"),1)

=IFS(OR(SUBSTITUTE($A1,"  ","")="]",SUBSTITUTE($A1,"  ","")="}"),1)



=IF(COUNTIF($A:$A,A1)>1,1,0)


=IF(LEFT(SUBSTITUTE($A1,"  ",""),2)="//",MID(SUBSTITUTE($A1,"  ",""),3,999),A1)

