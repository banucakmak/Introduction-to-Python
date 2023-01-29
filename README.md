# Introduction-to-Python
First lesson of the Datascience Bootcamp! I am getting to used to basics of pythonn!!

It includes examples from;
printing,
print("Merhaba Dünya")

python as a calculator,

![image](https://user-images.githubusercontent.com/122751581/215348250-2d86cf89-e3b6-4b0d-8914-dc9c12cc2b5f.png)

managing packages, 

import pandas as pd

reading data sets with various extensions from computer memory and website, 
df=pd.read_xml("catalog.xml")


some basic commands for exploratory data analysis, feature engineering and text audio output.

df.head()

plt.figure(figsize=(20,8))
sns.countplot(x=df["Notlar"]) 
plt.xticks(rotation=90);


df['Survived'].value_counts()
d={1.0:"Hayatta",0.0:"öldü"}
df['Survived']=df['Survived'].map(d)


from gtts import gTTS

text="Merhaba Zafer, Yapay zeka dersimizi nasıl buldunuz?"

output=gTTS(text=text,lang='tr', slow=False)

output.save('konusma.mp3')

from IPython.display import Audio
audio=Audio(filename='konusma.mp3')
audio
