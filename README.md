# SCNU SoCoding Open Source Mirror

华南师范大学软件协会开源镜像站。

目录存放的是镜像站使用的 NGINX FancyIndex 主题，修改自 [artyuum/Nginx-FancyIndex-Theme](https://github.com/artyuum/Nginx-FancyIndex-Theme/)。

安装好 FancyIndex 插件后，编辑配置文件：

```
location / {
    fancyindex on;
    fancyindex_localtime on;
    fancyindex_exact_size off;
    fancyindex_header "/Nginx-FancyIndex-Theme/header.html";
    fancyindex_footer "/Nginx-FancyIndex-Theme/footer.html"; 
    fancyindex_ignore "favicon.ico";
    fancyindex_ignore "Nginx-FancyIndex-Theme";
    fancyindex_name_length 255;
}
```

重启 NGINX 使配置生效。