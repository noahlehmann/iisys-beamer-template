# Iisys Tex Beamer Template

This is a LaTeX beamer template for the Iisys group at the University of Applied Sciences in Hof.

## Build the document

You can simply build the document with the provided Containerfile. 
Assuming you have [docker](https://docs.docker.com/get-started/get-docker/) installed already, just run the following command:

```bash
docker build --output type=local,dest=. --target pdf -f build/Containerfile .
```

The build process will take a while on first run as it needs to download the texlive distribution.
The resulting pdf will overwrite the `main.pdf` in the project base directory.

For convenience and easy automation in your IDE, the `run.sh` script is provided. 
It currently expects no arguments. 

```bash
./run.sh
```

## Font Sizes

With 12pt the fontsizes translate to the following sizes:

| command       | size  | 
|---------------|-------|
| \tiny         | 6pt   |  
| \scriptsize   | 8pt   |  
| \footnotesize | 10pt  | 
| \small        | 11pt  | 
| \normalsize   | 12pt  | 
| \large        | 14pt  | 
| \Large        | 17pt  | 
| \LARGE        | 20pt  | 
| \huge         | 25pt  | 
| \Huge         | 25pt  |
