[toc]

# wqiiqw 2025/07/17 notes

On Ubuntu 24.04: PRETTY_NAME="Ubuntu 22.04.5 LTS"


```
 export https_proxy=http://127.0.0.1:9910
 export http_proxy=http://127.0.0.1:9910
 python3 -m venv .venv
 source .venv/bin/activate
 pip install sphinx-simplepdf
 cd demo/
 pip install -r doc-requirements.txt
 pip uninstall -y pygls esbonio sphinx-needs
 pip install "pygls<1.0"
 pip install sphinx-needs esbonio
 pip show pygls | grep Version   # → Version: 0.13.1
 sphinx-build -a -E -b simplepdf . _build/   # should now run
```