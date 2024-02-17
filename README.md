# mofis-font
A Iosevka configuration

![image](https://github.com/mokrates/mofis-font/blob/main/mofis.png?raw=true)

## Download

See the github releases: https://github.com/mokrates/mofis-font/releases

## how to build

Clone the Iosevka git:

	git clone --depth 1 https://github.com/be5invis/Iosevka.git 

get `private-build-plans.toml` and `build.sh` from this git and copy
it into the `Iosevka` directory and run `build.sh`.

	git clone https://github.com/mokrates/mofis-font
	cp mofis-font/private-build-plans.toml mofis-font/build.sh Iosevka/
	cd Iosevka

	# if you don't have installed verda
	npm install verda
	bash build.sh
	
Your font will be
built into `Iosevka/dist`. Copy the resulting directory into `~/.fonts`.

## Which font to use

There are many variants generated. Usually I use the

    Mofis 0.4 Extended 
	
variant.

### Ligatures

If you want a font with programming ligatures, the font currently for you is

	Mofis 0.3 Extended
	
## Using the font

### Thunderbird

Thunderbird offers a font chooser which doesn't allow you to choose
`Mofis 0.4 Extended`, but only `Mofis 0.4` (or whatever version you
try to use). Choose this, and open the `about:config` ("Menu" ->
"Settings" -> scroll to the bottom and choose "edit Settings"). Search
for "font" and look for where `Mofis 0.4` is selected. These are just
string settings, so you can amend it to "Mofis 0.4 Extended"

### Emacs

`~/.emacs`
```
(add-to-list 'default-frame-alist
	     '(font . "Mofis 0.4 Extended-11"))
```

## License

The License is the SIL Open Font License v1.1 as used by Iosevka,
which I am not sure this is even a deriviate of, b/c this only is a
configuration using their customizer:
https://typeof.net/Iosevka/customizer
