Documenta como buscar os dados (exemplo com Roboflow):
```md
# 📦 Datasets - Smart Walker

Os datasets usados neste projeto são armazenados no **Roboflow**.  
⚠️ As imagens não são guardadas diretamente no GitHub para evitar ficheiros grandes.

## 🚀 Como descarregar

```python
from roboflow import Roboflow
rf = Roboflow(api_key="A_TUA_API_KEY")
project = rf.workspace("o_teu_workspace").project("walker-obstacles")
dataset = project.version(1).download("yolov8")
