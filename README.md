# CDN Detector

サイトのURLを入力すると、サイトが使用しているCDNがなにかを当ててくれます。
判定条件は[Wappalyzer](https://github.com/wappalyzer/wappalyzer)のものを使わせていただきました。

以下のようにしてローカルで使用できます。Python3.11で動作確認済みです。古いPythonを使用していると、パッケージのインストールに失敗することがあります。

```python3
git clone https://github.com/rihib/cdn-detector.git
cd cdn-detector
python3 -m venv .venv
source .venv/bin/activate
python3 -m pip install --upgrade pip
python3 -m pip install -r requirements.txt
python3 src/main.py
```

動作はかなり遅いです。CDNの名前が出てくるまで気長にお待ちください。
