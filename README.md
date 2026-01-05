结肠镜息肉分割常用数据集汇总仓库，包含 4 个经典公开数据集，使用 Git LFS 管理大文件。

📋 项目简介
本仓库收集了胃肠道内镜（结肠镜）息肉分割任务中常用的 4 个公开数据集，方便研究者快速获取、统一管理数据，适用于医学图像分割、计算机辅助诊断等学术研究场景。
包含数据集：
CVC-ClinicDB
CVC-ColonDB
ETIS-LaribPolypDB
Kvasir-SEG

📊 数据集列表
数据集名称	            任务类型	         模态	      数据量（图像 + 掩码）
CVC-ClinicDB	    结肠镜息肉分割	  结肠镜 RGB 图像	    612 幅
CVC-ColonDB	      结肠镜息肉分割	  结肠镜 RGB 图像	    380 幅
ETIS-LaribPolypDB	结肠镜息肉分割	  结肠镜 RGB 图像	    196 幅
Kvasir-SEG	      结肠镜息肉分割	  结肠镜 RGB 图像	   1000 幅

📂 各数据集详情
1. CVC-ClinicDB
来源：西班牙瓦伦西亚理工大学（Polytechnic University of Valencia, CVC）
任务：结肠镜图像中的息肉实例分割
数据特点：包含不同大小、形态的息肉，图像分辨率统一为 384×288
原始发布：用于 2015 年 MICCAI EndoScene 息肉检测竞赛
2. CVC-ColonDB
来源：西班牙瓦伦西亚理工大学（CVC）
任务：结肠镜息肉分割
数据特点：包含更多复杂背景的息肉图像，分辨率为 576×500
适用场景：适用于鲁棒性较强的分割模型测试
3. ETIS-LaribPolypDB
来源：法国 ETIS 实验室 + 埃及 Larib 实验室
任务：结肠镜息肉分割
数据特点：息肉占比更小、背景更复杂，分辨率为 768×576
难度：相对其他数据集难度更高
4. Kvasir-SEG
来源：挪威奥斯陆大学 + 医疗科技公司 Kvasir
任务：结肠镜息肉分割
数据特点：来自真实临床场景的多样化息肉图像，分辨率为 332×500
优势：数据量较大，贴近实际临床需求

🛠️ 使用方法
本仓库通过Git LFS管理大尺寸图像文件，请按照以下步骤获取数据：
先安装 Git LFS（已安装可跳过）：
bash
运行
# Ubuntu/Debian
sudo apt install git-lfs
# MacOS（Homebrew）
brew install git-lfs
# Windows：从Git LFS官网下载安装包
初始化 Git LFS：
bash
运行
git lfs install
克隆本仓库：
bash
运行
git clone [你的仓库URL]

📚 引用方式
若使用本仓库中的数据集，请引用各数据集的原始论文：
CVC-ClinicDB：
bibtex
@inproceedings{carneiro2015endoscene,
  title={EndoScene: A new dataset for polyp detection and classification},
  author={Carneiro, Gustavo and et al.},
  booktitle={MICCAI Workshop on Computer-Aided Detection and Diagnosis in Medical Imaging},
  year={2015}
}
CVC-ColonDB：
bibtex
@inproceedings{bernal2014segmentation,
  title={Segmentation of colorectal polyps with kernel density estimation and graph cuts},
  author={Bernal, Jorge and et al.},
  booktitle={IEEE International Symposium on Biomedical Imaging},
  year={2014}
}
ETIS-LaribPolypDB：
bibtex
@article{walk2017etis,
  title={ETIS-LaribPolypDB: A polyp dataset for computer aided diagnosis in colonoscopy},
  author={Walk, Simon and et al.},
  journal={Journal of Biomedical and Health Informatics},
  year={2017}
}
Kvasir-SEG：
bibtex
@article{jha2020kvasir,
  title={Kvasir-SEG: A segmented polyp dataset from gastrointestinal tract},
  author={Jha, Debesh and et al.},
  journal={Scientific Data},
  year={2020}
}

📜 许可证声明
各数据集遵循其原始发布许可证：
CVC-ClinicDB/CVC-ColonDB：学术非商用许可
ETIS-LaribPolypDB：CC BY-NC-SA 4.0
Kvasir-SEG：CC BY 4.0

⚠️ 免责声明
本仓库仅用于学术研究目的，不用于临床诊断或商用。使用数据时请遵守各数据集的原始使用条款，作者不对数据的准确性、适用性承担责任。
