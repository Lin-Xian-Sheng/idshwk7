信息嵌入/隐藏和提取步骤如下：
（1）准备好原图：original.png和待嵌入/隐藏的文本information.txt
（2）利用LSB算法进行文本嵌入/隐藏：python3 LSBSteg.py encode –i original.png -o test.png -f information.txt，即可得到已经嵌入/隐藏信息的图片test.png
（3）进行解码，验证图片中的嵌入/隐藏信息：python3 LSBSteg.py decode –i test.png –o decodeinfo.txt，即可得到嵌入/隐藏的文本decodeinfo.txt
（4）对比information.txt和decodeinfo.txt，可知成功嵌入和成功提取
