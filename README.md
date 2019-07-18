# EasySwipeMenuLayout
A sliding menu library not just for recyclerview, but all views.
# Effect picture
![EasySwipeMenuLayout.gif](http://upload-images.jianshu.io/upload_images/1811893-e1aa5b2f36f1caf5.gif?imageMogr2/auto-orient/strip)

# Recommended

- Recommended in conjunction with BaseRecyclerViewAdapterHelper

# Feature

- 1、Two-way sliding
- 2、Support any View
- 3、By id binding layout, more freedom

# How to use
## Step 1

- You need to add jitpack repository infomaition to build.gradle in your project.
        
        // Top-level build file where you can add configuration options common to all sub-projects/modules.
        buildscript {
            repositories {
                jcenter()
            }
            dependencies {
                classpath 'com.android.tools.build:gradle:2.2.0'
        
                // NOTE: Do not place your application dependencies here; they belong
                // in the individual module build.gradle files
            }
        }
        
        allprojects {
            repositories {
                jcenter()
                maven { url "https://jitpack.io" }
        
            }
        }
        
        task clean(type: Delete) {
            delete rootProject.buildDir
        }

## step 2

[![](https://jitpack.io/v/anzaizai/EasySwipeMenuLayout.svg)](https://jitpack.io/#anzaizai/EasySwipeMenuLayout)

- You need to add library dependencies infomation to build.gradle in your module.

      compile 'com.github.anzaizai:EasySwipeMenuLayout:1.1.4'

- last releases version is 1.1.4 can be use

## step 3
- User EasySwipeMenuLayout as the top-level root layout the needs to be added slide swipe menu the funcation views.
 
### such as
            <com.guanaj.easyswipemenulibrary.EasySwipeMenuLayout
                      android:layout_width="match_parent"
                      android:layout_height="wrap_content"
                      app:contentView="@+id/content"
                      app:leftMenuView="@+id/left"
                      app:rightMenuView="@+id/right">
                          <LinearLayout
                              android:id="@+id/left"
                              android:layout_width="100dp"
                              android:layout_height="wrap_content"
                              android:background="@android:color/holo_blue_dark"
                              android:orientation="horizontal"
                              android:padding="20dp">
                                  <TextView
                                        android:layout_width="wrap_content"
                                        android:layout_height="wrap_content"
                                        android:text="分享" />
                            </LinearLayout>
                          <LinearLayout
                              android:id="@+id/content"
                              android:layout_width="match_parent"
                              android:layout_height="wrap_content"
                              android:background="#cccccc"
                              android:orientation="vertical"
                              android:padding="20dp">
                                  <TextView
                                        android:layout_width="wrap_content"
                                        android:layout_height="wrap_content"
                                        android:text="内容区域" />
                          </LinearLayout>
                          <LinearLayout
                              android:id="@+id/right"
                              android:layout_width="wrap_content"
                              android:layout_height="wrap_content"
                              android:background="@android:color/holo_red_light"
                              android:orientation="horizontal">
                              <TextView
                                  android:layout_width="wrap_content"
                                  android:layout_height="wrap_content"
                                  android:background="@android:color/holo_blue_bright"
                                  android:padding="20dp"
                                  android:text="删除" />
                              <TextView
                                  android:id="@+id/right_menu_2"
                                  android:layout_width="wrap_content"
                                  android:layout_height="wrap_content"
                                  android:background="@android:color/holo_orange_dark"
                                  android:padding="20dp"
                                  android:text="收藏" />
                          </LinearLayout>
                    </com.guanaj.easyswipemenulibrary.EasySwipeMenuLayout>

- yes，just one step,use it is so simple
# Portal
- 想要阅读源码的小伙伴可以点击我的博客，在博客里简略分析了构建的思路我实现过程
- 个人博客：[https://www.catbro.cn](https://www.catbro.cn/)