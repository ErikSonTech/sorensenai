## Crear entorn i instal·lar dependències
```bash
conda create -n sorensenai python=3.10 -y
conda activate sorensenai
pip install -r requirements.txt
```

## Aixecar entorn
```bash
```

# Pre requisits

Al repo trobaràs un fitxer srt [subtitols_ca.srt](subtitols_ca.srt), correspon als subtítols del vídeo [https://www.youtube.com/watch?v=sm9wfoO_W1Q](https://www.youtube.com/watch?v=sm9wfoO_W1Q)

El video es pot descarregar usant yt-dlp (instal·lat via requirements):

```bash
yt-dlp -f "bestvideo+bestaudio" "https://www.youtube.com/watch?v=sm9wfoO_W1Q"
```

Amb el reproductor [VLC](https://www.videolan.org/vlc/) es pot veure el video juntament amb els subtítols.

# Què s'ha de fer?

Donats els subtitols mencionats anteriorment, s'ha d'aconseguir generar els mateixos subtítols en castellà (subtitols_es.srt) i en anglés (subtitols_en.srt).

La traducció resultant ha de tenir en compte el context, no ha de ser una traducció literal. Ha de seguir sincronitzat i ha de seguir sincronitzat en temps amb el video.

Com a punt de partida es pot usar el notebook d'aquest repo [traductor.ipynb](traductor.ipynb)


