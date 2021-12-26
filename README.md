Elaina ChatBot API
Để có thể ủng hộ câu từ cho API bạn có thể theo các bước như sau:

Bước 1:
Nhấn vào icon cây bút ở bên phải và thêm câu từ theo quy tắc sau:
intent: để chỉ tên của mục (không đặt trùng tên)
utterances là các câu người dùng hỏi bot
answers là phần bot sẽ reply lại

*Lưu ý: sử dụng ngôn từ phù hợp

Cách dùng API:
const key = "your_key"
let res = await axios.get(encodeURI(`https://api.elainateam.xyz/chatbot?key=${key}&msg=${message.content}`));
    if (!res.data.msg){
        return message.channel.send(`Tớ hong biết bạn đang nói j á`)
    }else{
        return message.channel.send(res.data.msg)
    }

Credit: 
Owner: Peter Tuan Anh, DiozVN
Admin: Tohru, CookieGMVN
Adder: The DT, PhatDev
