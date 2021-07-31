#Adobe usecase challenge 2
This is an implementation of the microsoft power automate flow for the following usecase designed for adobe usecase chanllenge 2

demo video link:https://youtu.be/XKv7O5JxcWU

##Usecase
You are a sales rep working for a big company and you need to come up with sales projects on a weekly basis.
You also need to manage the projects which is proposed by other people, and send them for final decision to CEO.

You are tired of managing and sending emails by yourself everyday, and you want to automate it somehow.

###Using power automate flow to automate:
By using power automate, you don't have to send the email yourselves anymore,
the daily flow is going to check for new projects which you think is ready to submit for approval in your one drive folder, and convert them 
to pdf format, then send them to your boss for approval.

You can even configure when this process happens so your mail is always going to be the most recent item when your boss checks his/her email box in the morning.

When your boss has signed the document, the second flow will trigger and you will automatically receive a copy of the signed document in your onedrive.
It will also keep the files in structured folders:
`ready`,`sent`,and `approved`.

All you need to do is create these 3 folders and the flow is going to keep everything clean.

##Usage of adobe connectors
Adobe tools api is used to transform word documents to pdf documents.

Adobe sign api is used to retrieve signed apis and to create agreements from the transformed pdf.
