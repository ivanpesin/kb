# ffmpeg tips and tricks

## Speed up video recording

Speed up video and audio x1.25:

`ffmpeg -i <input_file> -filter_complex "[0:v]setpts=PTS/1.25[v];[0:a]atempo=1.25[a]" -map "[v]" -map "[a]" <output_file>`
