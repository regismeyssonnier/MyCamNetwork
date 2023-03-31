# MyCamNetwork


# 1. MyCamNetwork

If you **_`push r`_** key, it detect me !!!!!! Add your own model to detect you with tensorflow !!!!!!!!

If you **_`push f`_**, it put some glass on your face !!!!!!!!!!!!!!!

Look at the code for more info !!!!!! 🤣 

Run the file mycam.py !!!!!! Made with python, openCV and tensorflow !!!!!!!!!


![glass](https://user-images.githubusercontent.com/67794100/223876074-aac23905-9642-4a18-af96-6c6e5e4cc775.png)

# 2. Create his own model

To create your own model (neural network).

Use the class MyNetwork: 

```python
    mynet = MyNetwork("regis", 180, 180, "image/copy")
    mynet.init_model(25, 0.2)
    mynet.create_model()  
    mynet.train_model(10)
    mynet.get_history()
    mynet.save_model("model/yournamemodel") 
```

# 3. Create your photo

Run **`mycam.py`**, modify a little the code if it dooesn't run like the path ...

Take your photo by pushing the **_`key p`_**, (key == 112 in the code). And train the model with it !!!

Take about ****250 photo**** of you in different angle, and **another category** of photo who is **_different of your face_**(😵‍💫 ).

Thus, you create your directory in image/yourname and the other category image/photodifferentofyou. This will be your dataset for the model.

# 4. Load the model

Uncomment this code in mynetwork.py(it is uncommented), and load the model with this code.

```python
    mynet = MyNetwork("regis", 180, 180, "image/copy")
    mynet.load_model("model/regismodel")
    mynet.predict("image/test.png")
```

# 5. Filter

Look at the Key code and try some fun filter like sobel, colored, canny, hough

# 6. Soon a game

Push **_`t key `_**and after that _****track your hand by a circle****_ who displays it. After again, push **_`g key`_**  

and try to _**catch the ball**_ or fight it by hittin' in that ball with **_`your tracked hand`_** !!!!!  

This is the game :

![cam](https://user-images.githubusercontent.com/67794100/225127107-801724d7-2d99-4530-b2b1-fea5ed4fd811.png)

# 7. Audio detection

With **_`MySound Class`_** in mysound.py **record your voice** in saying who is it, and with other sentence, to create a **neural network** 

who _**recognize your voice**_. To create the audio neural network use the **_`class MyAudio`_** in myaudio.py like that 👍 :`

This is the code for record your voice:

```python
    mysound = MySound("regis.wav")
    mysound.record(3, 16000, 1)
    mysound.wait()
    mysound.save()
    mysound.play()
```

And this is the code to create the model who will recognize your voice:

```python 
    myaudio = MyAudio("sound")
    myaudio.init_model(64)
    myaudio.create_model()
    myaudio.test_model()
    myaudio.save_model("model/audiomodel")
```

You have to create a **_`sound directory`_** with _**`subdirectory`**_ with the name of their **class** like for the image. 

For example, no, yes, or _**who**_ (for who is it sentence). Their subdirectory will store your voice record like i mention above.

In the application, you have to use the **_`d key`_** to do this job for using the voice recognition action. 

# 8. Soon an AI vocal

**_`Push b`_** and **_ask_** : "Mets le filtre s noir", ou "Mets le jeu", or other _**command**_ see in the code. 

And the assistant **answer** and put what you **asked in action**.

# Final

Run **_`mycam.py`_** to show that !!!!!!!!

PS: Don't forget to install **open-cv-contrib, spacy, vosk, gtts, playsound, sounddevice, scipy, tensorflow, matplotlib**...

 _**DON'T WORRY**_  see in the code or on the internet for help !!!!
