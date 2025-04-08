## 代码核心功能说明

### 1、用以读取文本并过滤无效字符和长度为1的词的函数；
    def get_words(filename)：
### 2、该函数用以遍历邮件建立词库后返回出现次数最多的词；
    def get_top_words(top_num)：
### 3、该函数用以对未知邮件分类。
    def predict(filename)：


## 高频词/TF-IDF两种特征模式
###
### 参数化实现思路
### 接口设计：
#### 定义全局参数 feature_type（如 'freq' 或 'tfidf'），通过条件判断选择特征提取器。
### 模块化封装：
#### 使用 sklearn.feature_extraction.text.TfidfVectorizer 实现TF-IDF加权。自定义 CountVectorizer + 词频排序实现高频词特征。
### 统一输出格式：
#### 确保两种方法返回相同维度的特征矩阵，避免下游模型接口不兼容。

## 代码运行结果
<img src="https://github.com/ropzz121/3.13/blob/main/images/Ropz_at_BLAST_Bounty_Spring_2025.jpg" width="200" alt="车主本人">