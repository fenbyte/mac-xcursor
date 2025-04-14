# mac-xcursor
a 1:1 port of the cursors from macos into the xcursor format for linux

## why this is better than the rest
it's not a remake, it's a port. i'm not using random inaccurate svgs i found online, or scaling the hidpi versions back down to lodpi, i sourced the original raster images found on the latest version of macos and used the exact same hotspots that macos does. this is the most accurate pixel-perfect port ever made for linux, as far as i'm aware. short of hidpi support, it doesn't get better than this

## how i made it
i used a mac app called [mousecape](https://github.com/alexzielenski/mousecape/releases) to dump all of the vanilla macos cursor to a gigantic ".cape" file, which is just a renamed xml plist. this file contains every cursor in macos in their original tiff format encoded in base64, along with their x and y hotspots and resolution. i decoded all of the base64 into individual files, sorted through which cursors i did and did not need, converted them to pngs, named them accordingly, and made .cursor files for each with the hotspots that macos uses

## why didn't i script this?
because i'm an idiot and figured it'd be faster to do it manually. i was probably wrong

## hidpi support?
i don't have the sanity for that, sorry. maybe if i ever personally have a need for hidpi versions i'll do it, but right now, no

## how to install?
download the zip from the releases page and put the mac-xcursor folder in ~/.icons. enabling it is dependant on your environment, but it's probably self explanitory

## hyprcursor support?
official svgs aren't available, so no

## windows support?
no

## macos support?
![a picture of a cake with "congration you done it" written in icing](https://files.catbox.moe/8kkms9.png)
