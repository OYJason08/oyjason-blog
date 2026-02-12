---
title: "Private Gallery"
date: 2026-02-11T23:38:00
description: "An encrypted gallery. Decryption happens purely on the client-side."
type: "gallery"
layout: "gallery"

# 侧边栏菜单配置
menu:
    main:
        weight: -90
        params:
            icon: photo # 确保你有对应的 photo.svg

# 加密资源列表
# 这些文件应存放在你的 static/gallery/ 目录下
images:
    - src: "/gallery_enc/photo1.jpg.enc"
    - src: "/gallery_enc/photo2.jpg.enc"
    - src: "/gallery_enc/photo3.jpg.enc"
    - src: "/gallery_enc/photo4.jpg.enc"
    - src: "/gallery_enc/photo5.jpg.enc"
    - src: "/gallery_enc/photo6.jpg.enc"
    - src: "/gallery_enc/photo7.jpg.enc"
    - src: "/gallery_enc/photo8.jpg.enc"
    - src: "/gallery_enc/photo9.jpg.enc"
    - src: "/gallery_enc/photo10.jpg.enc"

# 页面提示语
password_hint: "Enter the PBKDF2 derived key to reveal contents."
---

## 协议声明 (Protocol Protocol)

本相册采用 **AES-GCM-256** 加密算法。所有图像解密过程均在您的浏览器本地内存中完成，服务器不存储任何明文密钥或解密后的像素数据。

> **Warning**: 如果密码丢失，没有任何手段可以恢复这些受损的熵。