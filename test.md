test_orig.png是原始图片
liuyujie.png是个人信息
test.png是加密过的包含个人信息的图片
watermark是最终解密得到的水印

执行以下命令加密个人信息得到test.png
encode.py --image test_orig.png --watermark liuyujie.png --result test.png

执行以下命令解密得到水印watermark.png
decode.py --image test.png --orig test_orig.png --result watermark.png
