# imagesearcharea
Func _imagesearcharea
If NOT ($transparency = 0) Then $findimage = 
	If $tolerance > 0 Then $findimage = "*" 
	$result = DllCall("ImageSearchDLL.dll", "str",
	If $result[0] = "0" Then Return 0
	$array = StringSplit($result[0], "|")
	$x = Int(Number($array[2]))
	$y = Int(Number($array[3]))
	If $resultposition = 1 Then
		$x = $x + Int(Number-#
		$y = $y + Int(Number $#
	EndIf
	Return 1
