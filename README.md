Hola ya existo
# instalacion de ollama
curl -fsSL https://ollama.com/install.sh | sh

# Ejecutar el servidor
ollama serve

# Paso 3
ollama pull tinyllama

# Hola mundo(porque el cielo es aazul)
curl http://localhost:11434/api/generate -d '{
  "model": "tinyllama",
  "prompt":"Porque el cielo es azul?"
}'

curl http://localhost:11434/api/generate -d '{
  "model": "tinyllama",
  "prompt": "Porque el cielo es azul?",
  "stream": false
}'

