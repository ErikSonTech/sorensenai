# Pre requisits

# Instal·lar anaconda

## Crear entorn i instal·lar dependències

```bash
conda create -n sorensenai python=3.10 -y
conda activate sorensenai
pip install -r requirements.txt
```

## Aixecar entorn

```bash
conda activate sorensenai
```

## Passos a seguir

Passos a seguir
Al repo trobaràs un fitxer srt [subtitols_ca.srt](subtitols_ca.srt), correspon als subtítols del vídeo [https://www.youtube.com/watch?v=sm9wfoO_W1Q](https://www.youtube.com/watch?v=sm9wfoO_W1Q)

El video es pot descarregar usant yt-dlp (instal·lat via requirements):

```bash
yt-dlp -f "bestvideo+bestaudio" "https://www.youtube.com/watch?v=sm9wfoO_W1Q"
```

Amb el reproductor [VLC](https://www.videolan.org/vlc/) es pot veure el video juntament amb els subtítols.

# Què s'ha de fer?

Donats els subtitols mencionats anteriorment, s'ha d'aconseguir generar els mateixos subtítols en castellà (subtitols_es.srt) i en anglés (subtitols_en.srt).

La traducció resultant ha de tenir en compte el context, les frases anteriors i posteriors, no ha de ser una traducció literal i ha de seguir sincronitzat  amb el video.

Com a punt de partida es pot usar el notebook d'aquest repo [traductor.ipynb](traductor.ipynb)

**Important**
Fer-ho amb el menor número de crides possibles a la API. Com a dada, es pot resoldre amb una sola crida. Seria acceptable fer-ho **amb 5 o menys crides**.

Et proporcionarem una API Key d'OpenAI.

Un cop finalitzat, envia'ns un zip amb el codi i els fitxers srt resultants.
