# Solana

## Solana programing philosophy

Về lý thuyết solana giống như unix system, nơi mọi thứ đều là file. Đối với solana thì là #account.

## Account

#account là đơn vị lưu trữ của solana, giống như file. Account chứa data hoặc bytecode. Nếu là bytecode thì nó sẽ trở thành #program. Mỗi #account đều phải có owner là một #program. Còn bản thân #program, owner của nó là #system_program. 

#program được thực thi bới #system_program, thông qua BPF loader.