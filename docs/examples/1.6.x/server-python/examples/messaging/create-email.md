from appwrite.client import Client

client = Client()
client.set_endpoint('https://cloud.appwrite.io/v1') # Your API Endpoint
client.set_project('<YOUR_PROJECT_ID>') # Your project ID
client.set_key('<YOUR_API_KEY>') # Your secret API key

messaging = Messaging(client)

result = messaging.create_email(
    message_id = '<MESSAGE_ID>',
    subject = '<SUBJECT>',
    content = '<CONTENT>',
    topics = [], # optional
    users = [], # optional
    targets = [], # optional
    cc = [], # optional
    bcc = [], # optional
    attachments = [], # optional
    draft = False, # optional
    html = False, # optional
    scheduled_at = '' # optional
)