# grid-ginkgo
repeatable tests of Grid.ai CLIs


# Setup
```bash
brew install golang

go get github.com/onsi/ginkgo/ginkgo
go get github.com/onsi/gomega/...
 
cat >> ~/.zshrc <<'EOF'
export GOPATH=$HOME/go
export GOROOT=/usr/local/opt/go/libexec
export PATH=$PATH:$GOPATH/bin
export PATH=$PATH:$GOROOT/bin
EOF
```

# boot strap

```bash
mkdir -p $GOPATH/src
cd $GOPATH/src
git clone https://github.com/robert-s-lee/grid-ginkgo
cd grid-ginkgo
ginkgo bootstrap
```