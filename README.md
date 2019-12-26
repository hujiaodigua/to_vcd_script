采集数据得到data.txt指令 
-- ./main data.txt
处理data.txt得到mailbox_samples.txt指令
-- python3 file_bin2hex.py
处理mailbox_samples.txt得到mailbox_samples.vcd指令
-- python3 pyusb_sample_fx2_vcd.py mailbox_samples.txt >> mailbox_samples.vcd

注意需要安装pyvcd库
C:\Users\Administrator\AppData\Local\Programs\Python\Python36\Lib\site-packages\vcd 路径下的writer.py文件 TIMESCALE_NUMS里加上采样率MHz对应的时间