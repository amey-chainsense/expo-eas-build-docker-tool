docker build -t my-expo-app .
docker run -it --rm --name my-running-app -v "$PWD":/app -w /app my-expo-app bash

expo login

git config --global user.name username
git config --global user.email user@mail.com

git config --global --add safe.directory /app

eas build --profile development --platform android --local

eas build --platform android --local
docker cp my-running-app:/app/build-1722961016133.aab build/
