# flaskappthroughazure
While solutions using machine learning or artificial intelligence have become increasingly common, they can still be difficult to create from scratch. Fortunately, there are many solutions already built, which we can access like we would any application programming interface (API). This approach allows us to focus on our code, rather than complex modeling.

Azure provides a set of offerings called Cognitive Services, which include services for computer vision, speech to text and text to speech, and text translation. You can access any of these services via software developer kits (SDKs), or by calling them in the same way you'd call any other HTTP endpoint.

To use Cognitive Services, you'll need an Azure account. If you're new to Azure, you can sign-up for free, which will include $200 free credit for the first 30 days. If you're a student, you can enroll for Azure for Students, which includes $100 to use across 12 months, and a host of other free services.

Translator service
Translator service, part of Cognitive Services, will translate to and from dozens of languages. It can automatically detect the source language, and can translate to multiple target languages in one call. You call Translator service in the same way you would call any other HTTP endpoint. In Python, you typically do this by using the requests library, which is what we'll use when we return to our code.

Key management
To call Translator service (or any other Cognitive Service), we'll need a key. This key will be used whenever we access the service. The key is similar to a password. Anyone who has access to the key can call the service, and if we were using a paid version they could run up a large bill!

One great solution for protecting the key when doing development work is to use a library called python-dotenv, commonly called dotenv. When using dotenv, we create a file named .env, which contains any key/value pairs we don't want as part of our source code. We'll ensure that the file is listed in our gitignore file when we push our code to GitHub, so that we don't accidentally publish it for the world to see.
