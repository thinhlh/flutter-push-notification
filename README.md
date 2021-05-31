# Flutter Push Notification
> Flutter Application integrating cloud messaging provided by Firebase

To send push notification to the installed app, call the following **POST** request

- Endpoint
`https://fcm.googleapis.com/fcm/send/`

- Header
```
content-type: application/json```
Authorization: key= [key-will-be-specified-in-log-with-server-token tag]
```
- Body
Follow JSON snippet
```
{
	"to": "/topics/topic",
	"notification": {
		"title": "General notification",
		"body": "Dismissible"
	},
	"data": {
		"title": "In app notification",
		"body": "Undismissible, generally used for service requirements"
	}
}
```
