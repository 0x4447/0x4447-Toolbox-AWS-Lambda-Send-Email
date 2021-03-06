# 0x4447 AWS Lambda Send Email

The purpose of this AWS Lambda function is to quickly add email sending capabilities to your project. Once deployed you can invoke this function with the following payload:

```
{
    from        : '"First Last" <name@example.com>',
    to          : 'name@example.com',
    subject     : 'Nice subject',
    reply_to    : 'name@example.com'                    || '',
    html        : '<p>HTML version of the message</p>'  || '',
    text        : 'Plaintext version of the messag'     || ''
}
```

The function will return the `messageId` and `response` so you can log the ID of the sent email

```
{
    messageId: '<000000000000000000000000000@email.amazonses.com>',
    response: '0000000000000-0000-000-000-000-000-000000' 
}
```

# IAM Role

For the function to work you'll need to create a Role with the following policies:

- AWSLambdaBasicExecutionRole
- AmazonSESFullAccess

# The End

If you enjoyed this project, please consider giving it a 🌟. And check out our [0x4447 GitHub account](https://github.com/0x4447), where we have additional resources that you might find useful or interesting.

# For Hire 👨‍💻 👩‍💻

If you'd like us to help you with something, please feel free to say [hello@0x4447.email](mailto:hello@0x4447.email?Subject=Hello%20From%20Repo&Body=Hi%2C%0A%0AMy%20name%20is%20NAME%2C%20and%20I%27d%20like%20to%20get%20in%20touch%20with%20someone%20at%200x4447.%0A%0AI%27d%20like%20to%20discuss%20the%20following%20topics%3A%0A%0A-%20LIST_OF_TOPICS_TO_DISCUSS%0A%0ASome%20useful%20information%3A%0A%0A-%20My%20full%20name%20is%3A%20FIRST_NAME%20LAST_NAME%0A-%20My%20time%20zone%20is%3A%20TIME_ZONE%0A-%20My%20working%20hours%20are%20from%3A%20TIME%20till%20TIME%0A-%20My%20company%20name%20is%3A%20COMPANY%20NAME%0A-%20My%20company%20website%20is%3A%20https%3A%2F%2F%0A%0ABest%20regards.), and share what's on your mind. We'll take a look, and try our best to help you. Or visit our website at: [0x4447.com](https://0x4447.com).
