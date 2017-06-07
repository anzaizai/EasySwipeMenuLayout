# EasySwipeMenuLayout
A sliding menu library not just for recyclerview, but all views.

# 效果图
![EasySwipeMenuLayout.gif](http://upload-images.jianshu.io/upload_images/1811893-e1aa5b2f36f1caf5.gif?imageMogr2/auto-orient/strip)

# 特性
- 1、随心所欲的双向滑动
- 2、id绑定，更加自由
# 使用步骤
## 1、在布局文件中添加菜单布局，通过id绑定
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

- yes，只有一步，只需一步 
# 传送门
- 想要阅读源码的小伙伴可以点击我的博客，在博客里简略分析了构建的思路我实现过程
- 个人博客：[http://www.cherylgood.cn](http://www.cherylgood.cn/)