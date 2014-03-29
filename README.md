
###一百行golng代码写一个静态文件服务器

####包含功能 

1. 静态文件模板
2. 文件上传
3. 文件查看和下载

####使用的包

	import (
		"fmt"
		"html/template"
		"io"
		"net/http"
		"os"
		"path/filepath"
		"regexp"
		"strconv"
		"time"
	)

####包含知识点

	//静态文件服务器
	http.FileServer(http.Dir("目录"))

	//手工配置服务和路由
	s := &http.Server{
		Addr:           ":8080",
		Handler:        myHandler,
		ReadTimeout:    10 * time.Second,
		WriteTimeout:   10 * time.Second,
		MaxHeaderBytes: 1 << 20,
	}

	s.ListenAndServe();

	// path/filepath包的使用

麻雀虽小，但是有很多基础知识点适合学习golang的朋友们一起玩

###One hundred lines of code write a golang static server

####Contains functions 

1. static file temlate 
2. upload file
3. To view and download files

####the use pkg

	import (
		"fmt"
		"html/template"
		"io"
		"net/http"
		"os"
		"path/filepath"
		"regexp"
		"strconv"
		"time"
	)

####Contains the knowledge

	//static server
	http.FileServer(http.Dir("目录"))

	//Manually configure the service and routing
	s := &http.Server{
		Addr:           ":8080",
		Handler:        myHandler,
		ReadTimeout:    10 * time.Second,
		WriteTimeout:   10 * time.Second,
		MaxHeaderBytes: 1 << 20,
	}

	s.ListenAndServe();

	// path/filepath The use of the package 

The sparrow is small, but there are a lot of basic knowledge for learning golang friends to play together

