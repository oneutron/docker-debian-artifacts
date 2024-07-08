# Docker Debian Artifacts

## Clone Debian Bullseye
```sh
# Clone Repository https://github.com/debuerreotype/docker-debian-artifacts
# Directory bullseye

git clone --filter=blob:none --no-checkout https://github.com/debuerreotype/docker-debian-artifacts.git
cd docker-debian-artifacts
git sparse-checkout set --cone
echo "bullseye/" > .git/info/sparse-checkout
git checkout dist-amd64
mv bullseye ../dist-amd64
cd ..
rm -rf docker-debian-artifacts
git clone --filter=blob:none --no-checkout https://github.com/debuerreotype/docker-debian-artifacts.git
cd docker-debian-artifacts
git sparse-checkout set --cone
echo "bullseye/" > .git/info/sparse-checkout
git checkout dist-arm64v8
mv bullseye ../dist-arm64v8
cd ..
rm -rf docker-debian-artifacts
ls -alh
```
## Clone Debian Bookworm
```sh
# Clone Repository https://github.com/debuerreotype/docker-debian-artifacts
# Directory bookworm

git clone --filter=blob:none --no-checkout https://github.com/debuerreotype/docker-debian-artifacts.git
cd docker-debian-artifacts
git sparse-checkout set --cone
echo "bookworm/" > .git/info/sparse-checkout
git checkout dist-amd64
mv bookworm ../dist-amd64
cd ..
rm -rf docker-debian-artifacts
git clone --filter=blob:none --no-checkout https://github.com/debuerreotype/docker-debian-artifacts.git
cd docker-debian-artifacts
git sparse-checkout set --cone
echo "bookworm/" > .git/info/sparse-checkout
git checkout dist-arm64v8
mv bookworm ../dist-arm64v8
cd ..
rm -rf docker-debian-artifacts
ls -alh
```