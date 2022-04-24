# Slow-doubleclick
closecounter = 1 And TimerDiff($TimeHandle) &lt;= $closingdelay Then                 GUIDelete()                 Exit             EndIf             If $closecounter = 0 Then                 $closecounter = 1                 $TimeHandle = TimerInit()                 WinSetTitle($Form1, "", "Slow doubleclick to close")             EndIf         Case $typ = "loop"
