# XToolsLib

## v0.1

### Download

``` python
pip install XToolsLib
``` 

### Fake Mail

``` python
import XToolsLib, time

m = []

fm = XToolsLib.FakeMail()
email = fm.Create()

print("Your mail is : "+email)
print("_____________________\n")
while True:
	time.sleep(5)
	msg = fm.Messages()
	if len(msg) != 0 and not msg[0] in m:
		mm = msg[0]
		print("New message 📧")
		print("_____________________")
		print(f"Email : {mm['from']['address']}")
		print(f"Name : {mm['from']['name']}")
		print(f"Subject : {mm['subject']}")
		print(f"Message : {mm['message']}")
		print(f"Date : {mm['date']}")
		print("_____________________\n")
		m.append(mm)	
```

### Contact
Telegram : [Mr.Abood](https://t.me/O0O0I)

Channel : [X | Tools](https://t.me/O0OO2)

Email : XTools@outlook.sa

Project Link : https://github.com/Mr-Abood/XToolsLib
