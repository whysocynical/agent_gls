# 镜助理 - 智能人脸识别助手

## 项目说明

这是一个基于荧光绿风格的人脸识别应用,用于识别人员信息并显示相关资料。

## 使用步骤

1. **添加人脸图片**: 将需要识别的人脸图片放置在项目根目录下,例如 `图片1.png`
2. **配置人员信息**: 在 `index.html` 的 `faceDatabase` 对象中配置对应人员信息
3. **设置API Key**: 打开应用,进入"API设置",输入豆包视觉API Key
4. **开始识别**: 点击"开始识别",将摄像头对准人脸进行识别

## 人脸库配置

在 `index.html` 中找到 `faceDatabase` 对象,按以下格式添加人员信息:

```javascript
const faceDatabase = {
    '图片1.png': {
        name: '姓名',
        college: '所属学院',
        major: '专业',
        grade: '年级',
        studentId: '学号',
        bio: '个人简介',
        noticeTitle: '申报事项',
        noticeContent: '申报截止时间'
    },
    // 可以继续添加更多图片和人员信息
    '图片2.png': {
        // ...
    }
};
```

## API Key 获取

1. 访问火山引擎官网
2. 开通豆包视觉API服务
3. 创建并复制API Key

## 注意事项

- 请通过本地服务器(如 VS Code Live Server)访问,不要直接双击打开HTML文件
- 确保摄像头权限已授予
- 人脸图片建议清晰可见,正面人脸
- 需要HTTPS或localhost环境才能使用相机功能
