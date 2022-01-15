from pytube import YouTube
import os


link=input("İndirmek istediyiniz vidyonun linkini giriniz:")
directory = input("Visyonun indirmek istediyiniz adı giriniz:")

print("lütfen bekleyin")

try:
    yt=YouTube(link)
except:
    print("link is not valid")
    exit()
mp3 = yt.streams.filter(only_audio=True).first()


print("downloading...")

output = mp3.download(directory)

base, ext = os.path.splitext(output)
to_mp3 = base + ".mp3"
os.rename(output, to_mp3)

print("download complete")

//
