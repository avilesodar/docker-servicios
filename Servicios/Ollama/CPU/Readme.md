docker build -t ollama .

docker run -d -v ollama:/root/.ollama -p 11434:11434 --name ollama-ai ollama