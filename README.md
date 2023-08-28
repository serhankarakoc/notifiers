# notifiers
Golang Notifiers Paketi
# Kullanım
```
package main

import "notifiers"

func main() {
	server.Server()
	service := notifiers.NotificationService{}

	smsContent := map[string]string{"phone": "123456789", "content": "This is an SMS"}
	emailContent := map[string]string{"email": "example@example.com", "title": "Email Title", "content": "This is an email"}
	notificationContent := map[string]string{"title": "Notification Title", "content": "This is a notification"}

	service.Send("sms", smsContent)
	service.Send("email", emailContent)
	service.Send("notification", notificationContent)
}
```
