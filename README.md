# .bashrc
```
# ~/.bashrc

alias l="ls -1"
memp(){
    smem -t -k -c pss -P $1 | tail -n1;
}
get_audio_duration() {
    local audio_file="$1"

    if [[ -z "$audio_file" ]]; then
        echo "Usage: get_audio_duration <audio_file>"
        return 1
    fi

    if ! command -v ffprobe &> /dev/null; then
        echo "ffprobe is not installed. Please install FFmpeg."
        return 1
    fi

    local duration
    duration=$(ffprobe -i "$audio_file" -show_entries format=duration -v quiet -of csv="p=0" 2>/dev/null)

    if [[ -z "$duration" ]]; then
        echo "Failed to get the duration of the audio file."
        return 1
    fi

    echo "Duration: $duration seconds"
}
```


# .gitconfig

```
# ~/.gitconfig

[alias]
        st = status
        hist = log --pretty=format:'%C(white)%h %C(yellow)%cd %C(blue)%ce: %C(green)%s' --abbrev=8 --date=format:'%y-%m-%d %H:%M' -n20
	df = diff
	dfs = diff --staged
	ch = checkout
	cm = commit -m
```
