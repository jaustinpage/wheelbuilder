# wheelbuilder
Run this with a requirements.txt, and it will build your wheels. Use apk-requirements.txt to add dev packages that you might need. The wheels will be placed in the wheelhouse folder.  docker run -e REQUIREMENTS="$(cat requirements.txt)" -e APK_ADD="$(cat apk-requirements.txt)" -v "$PWD/wheelhouse:/wheelhouse" jaustinpage/wheelbuilder:latest
