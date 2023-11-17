# nicegui_qianfan_ai_chat

https://github.com/zauberzeug/nicegui/tree/main/examples/chat_with_ai

sudo docker run -it --restart always -p 1280:8080 -e PUID=$(id -u) -e PGID=$(id -g) -v $(pwd)/:/app/ zauberzeug/nicegui:latest

1、计费
https://cloud.baidu.com/doc/WENXINWORKSHOP/s/Blfmc9dlf

2、sdk调用
https://github.com/baidubce/bce-qianfan-sdk

pip install qianfan

3、依赖
langchain>=0.0.142
nicegui
openai
qianfan

4、坑人地方哈

os.environ["QIANFAN_AK"] = API_KEY
os.environ["QIANFAN_SK"] = SECRET_KEY

其实所谓的AK，不是access_token，就是app应用的API_KEY，调试了许久都不行，真的坑，多写几个字会死？？
