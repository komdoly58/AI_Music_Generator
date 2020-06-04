<h1>AI Music Generator</h1>

<p align="justify">
This is a Deep Learning & Natural Language Processing model which can generate Piano Music
</p>

<h2 id="intro">Introduction</h2>
<p align="justify">
The usage of Neural Networks has been steadily increasing over time. With a multitude of papers being published every year on this subject, Deep Learning has found its applications in many fields of our daily lives - ranging from recommedation systems and personalization to medical diagnosis and healthcare. A recently popularised area of applying these techniques is for content generation.
<br>
Text Generation, the most commonly seen form of this has become a ubiquitous feature in recent years. Auto-complete features in our message apps, emails and even Google searches is a common and helpful application of these methods. The model on the backend inputs and processes the few words typed by us and predicts the next most probable word from its vocabulary. The user has an option to use this word or continue typing, either of which further trains the algorithm as the model learns from the actual next word.
<br>
An attempt along a similar philosophy can be made to train a neural network to generate music, and this is indeed becoming popular in recent years. Here I build a Long-Short Term Memory (LSTM) neural network in Python using Keras, to generate piano music.
</p>

<h2 id="dataset"> Dataset </h2>
<p align="justify">
The dataset (contained in the /songs directory) consists of around 90 MIDI (Musical Instrument Digital Interface) audio files. Each of these files is a couple of minutes in duration and consists of piano music. Most of these files contain music from the Final Fantasy series of games, since the music is very distinct and has beautiful melodies. For playing the music of a file, follow the steps in <a href="#usage">Usage</a> section below.
</p>

<h2 id="model">Model</h2>
    <div align="center">
    <figure>
        <img src="model_plot.png"
             alt="Model Plot"
             width=400>
        <figcaption> A plot of the model and its layers </figcaption>
    </figure>
    </div>
    <p align="justify">
    I built an LSTM model using Keras Sequential API, which inputs sequences (of notes) of fixed length, and learns to predict the next note in the sequence. A summary of the model and a plot of its layers in given below -
    </p>
    
<h2 id="usage">Usage</h2>
<ol>
    <li>
        Install all dependencies
        <br>
        <code> pip install python3 </code>
        <br>
        <code> pip install numpy </code>
        <br>
        <code> pip install tensorflow </code>
        <br>
        <code> pip install keras </code>
        <br>
        <code> pip install timidity </code>
        <br>
        <code> pip install pickle-mixin </code>
        <br>
        <code> pip install music21 </code>
        <br>
        <code> pip install glob2 </code>
    </li>
    <li>
        Clone the repository to your system and head over to it <br>
        <code> git clone https://github.com/matakshay/AI_Music_Generator</code> <br>
        <code> cd AI_Music_Generator </code>
    </li>
    <li>
        To listen to a music file - <br>
        <code> cd songs </code> <br>
        <code> timidity [filename] </code> <br>
        Replace [filename] with complete name of file you wish to listen
    </li>
</ol>

<h2 id="acknowledgement">Acknowledgement</h2>
<p align="justify">
I referred many articles, blogs and websites while building this project, some of them are mentioned below-
</p>
    <ul>
        <li> https://colah.github.io/posts/2015-08-Understanding-LSTMs/ </li>
        <li> https://towardsdatascience.com/how-to-generate-music-using-a-lstm-neural-network-in-keras-68786834d4c5 </li>
        <li>https://en.wikipedia.org/wiki/Musicology</li>
        <li>https://en.wikipedia.org/wiki/Music_theory#Fundamentals_of_music</li>
        <li>https://en.wikipedia.org/wiki/Elements_of_music</li>
        <li>https://en.wikipedia.org/wiki/Definition_of_music</li>
    </ul>