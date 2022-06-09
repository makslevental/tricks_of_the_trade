# tricks_of_the_trade
Various QoL snippets and notes. YMMV.

## Install (Ubuntu) `ccache` for faster C++ compiles

Stolen from [https://askubuntu.com/a/470636](https://askubuntu.com/a/470636)

```bash
# Install package
sudo apt install -y ccache

# Update symlinks
sudo /usr/sbin/update-ccache-symlinks

# Prepend ccache into the PATH
echo 'export PATH="/usr/lib/ccache:$PATH"' | tee -a ~/.bashrc

# Source bashrc to test the new PATH
source ~/.bashrc && echo $PATH

which g++ gcc clang clang++
```



