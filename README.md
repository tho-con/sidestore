# Provision

English ⋅ [Français](LISEZMOI.md)

> **Warning**  \
> Don't use your main Apple account! Prefer a secondary Apple account.  \
> I am NOT responsible if something happens with your Apple account.

## What is this ?

a custom anisette server for sidestore, the cooler altstore. the below is straight from the official repo

## Dependecies

At runtime, libprovision requires some Apple libraries to be next to the executables. You should
download Apple Music APK (or just the architecture slice for your device if you prefer), and extract
the lib/ folder next to the executables. If you want to reduce further the size, you can remove in the lib/
folder all the libraries except libstoreservicescore.so and libCoreADI.so, since they are the only one
needed to run the app.

To build any of these projects, you need the D SDK, with the compiler and dub. As an option, you can also use libplist.

## Compilation

Clone the project and compile it with DUB:

```bash
git clone https://github.com/Dadoum/Provision --recursive
cd Provision
dub build -b release
```

or with CMake:

```bash
git clone https://github.com/Dadoum/Provision --recursive
cd Provision
mkdir build
cd build
cmake -G Ninja .. -DCMAKE_BUILD_TYPE=Release 
ninja
```

## Support

Donations are welcome with GitHub Sponsor.
