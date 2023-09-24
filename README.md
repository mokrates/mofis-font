# mofis-font
A Iosevka configuration

## how to build

Clone the Iosevka git:

    git clone https://github.com/be5invis/Iosevka/

get `private-build-plans.toml` and `build.sh` from this git and copy
it into the `Iosevka` directory and run `build.sh`.

	git clone https://github.com/mokrates/mofis-font
	cp mofis-font/private-build-plans.toml mofis-font/build.sh Iosevka/
	cd Iosevka
	bash build.sh
	
Your font will be
built into `Iosevka/dist`. Copy the resulting directory into `~/.fonts`.

## Which font to use

There are many variants generated. Usually I use the

    Mofis 0.1 Extended 
	
variant.

## License

The License is the SIL Open Font License v1.1 as used by Iosevka,
which I am not sure this is even a deriviate of, b/c this only is a
configuration using their customizer:
https://typeof.net/Iosevka/customizer
