{}は削除する

# Pythonの Version管理(pyenv)
pyenv にある python のバージョン確認  
```pyenv versions```

グローバル環境の設定  
```pyenv global {python-version}```

ローカル環境の設定  
```pyenv local {python-version}```

pyenv で設定した version の解除  
```pyenv {local or global} --unset```


# 仮想環境の設定(venv)
仮想環境の作成  
```python -m venv {env-name}```

仮想環境の実行  
```source ./{env-name}/bin/activate ```

pip installすると
./lib/{python-version}/site-packages
にデータが保存される。