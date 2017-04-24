# Android自定开发规范</br>
## 基本规范：</br>
* 方法通用</br>
•在允许函数重载的语言中，所有重载都应该执行相似的函数。</br>
•在变量名中使用互补对，如min/max、begin/end和open/close。</br>
•初始化方法，命名以init开头，例：initView</br>
•按钮点击方法，命名以to开头，例：toLogin</br>
•设置方法，命名以set开头，例：setData</br>
•具有返回值的获取方法，命名以get开头，例：getData</br>
•通过异步加载数据的方法，命名以load开头，例：loadData</br>
•布尔变量名应该含有is或has，或具有逻辑意义的单词，如：fileIsFound，hasSDcard</br>
•常量命名全部为大写单词，单词之间用下划线分开.如：public final static int PAGE_SIZE = 20;</br>
•在eclipse中使用Ctrl+shift+F格式化代码。</br>
•在Android studio 中使用Ctrl+shift+L格式化代码。</br>
•文字大小的单位统一用sp，控件大小的单位统一用dp。</br>
•应用中的字符串统一在strings.xml中定义，然后在代码和布局文件中引用。</br>
•颜色值统一在colors.xml中定义，然后在代码和布局文件中引用。（不要用系统的颜色）</br>
## 注释规范：</br>
* 文件头注释</br>
  文件顶部统一添加版权声明，声明的格式如下：</br>


      /**
       * Copyright (c) 2016.作者 Inc. All rights reserved.
       */
 
* 类和接口注释</br>
  类和接口统一添加javadoc注释，格式如下：</br>


      /**
        *  类或接口的描述信息
        
        *  @author ${作者}
        
        *  @date ${时间}.
        
        */

 * 方法注释</br>
  下面几种方法，都必须添加javadoc注释，说明该方法的用途和参数说明，以及返回值的说明。</br>
  •接口中定义的所有方法</br>
  •抽象类中自定义的抽象方法</br>
  •抽象父类的自定义公用方法</br>
  •工具类的公用方法</br>



         /**
           *  登录
           
           *  @param loginName 登录名
           
           *  @param password  密码
           
           *  @param listener  回调监听器
           
           */
 
 
       public void login(String loginName, String password, ActionCallbackListener<Void> listener);
      
      
      
* 变量和常量注释</br>

下面几种情况下的常量和变量，都要添加注释说明，优先采用右侧//来注释，若注释说明太长则在上方添加注释。</br>
•接口中定义的所有常量</br>
•公有类的公有常量</br>
•枚举类定义的所有枚举常量</br>
•实体类的所有属性变量</br>

      public static final int TYPE_CASH = 1; // 现金券
      public static final int TYPE_DEBIT = 2; // 抵扣券
      public static final int TYPE_DISCOUNT = 3; // 折扣券

      private int id;                // 券id
      private String name;           // 券名称
      private String introduce;      // 券简介
     
## 命名规范</br>
* 包命名：</br>
•基类、配置类、Application放在.base包下</br>
•Activity类统一放在.ui包下</br>
•fragment类统一放在.ui.fragment包下</br>
•service类统一放在.service包下</br>
•adapter类统一放在.adapter包下</br>
•工具类及其他统一放在.util包下</br>
•接口实现类统一放在.implement包下</br>
•封装的数据对象统一放在.bean包下</br>
•自定义的控件统一放在.view包下</br>
* 布局文件layout命名</br>
统一以 组件类型_功能 的格式命名，如：</br>
•activity_功能，为Activity的命名格式</br>
•fragment_功能，为Fragment的命名格式</br>
•dialog_功能，为Dialog的命名格式</br>
•item_list_功能，为ListView的item命名格式</br>
•item_grid_功能，为GridView的item命名格式</br>
•header_list_功能，为ListView的HeaderView命名格式</br>
•footer_list_功能，为ListView的FooterView命名格式</br>
* 控件引用字符串Strings的命名</br>
  类型_功能，如：</br>
  •页面标题，命名格式为：title_页面</br>
  •按钮文字，命名格式为：btn_按钮事件</br>
  •标签文字，命名格式为：label_标签文字</br>
  •选项卡文字，命名格式为：tab_选项卡文字</br>
  •消息框文字，命名格式为：toast_消息</br>
  •编辑框的提示文字，命名格式为：hint_提示信息</br>
  •图片的描述文字，命名格式为：desc_图片文字</br>
  •对话框的文字，命名格式为：dialog_文字</br>
  •menu的item文字，命名格式为：action_文字</br>
* colors的命名</br>
  前缀_控件(范围)，控件和范围选一个。</br>
  •背景颜色，添加bg前缀</br>
  •文本颜色，添加text前缀</br>
  •分割线颜色，添加div前缀</br>
  •区分状态时，默认状态的颜色，添加normal后缀</br>
  •区分状态时，按下时的颜色，添加pressed后缀</br>
  •区分状态时，选中时的颜色，添加selected后缀</br>
  •区分状态时，不可用时的颜色，添加disable后缀</br>
* drawable的命名</br>
前缀_控件(范围)</br>
•图标类，添加ic前缀</br>
•背景类，添加bg前缀</br>
•分隔类，添加div前缀</br>
•默认类，添加def前缀</br>
•区分状态时，默认状态，添加normal后缀</br>
•区分状态时，按下时的状态，添加pressed后缀</br>
•区分状态时，选中时的状态，添加selected后缀</br>
•区分状态时，不可用时的状态，添加disable后缀</br>
•多种状态的，添加selector后缀（一般为ListView的selector或按钮的selector）</br>
* 动画文件命名</br>
动画类型_动画方向,如：</br>
•fade_in，淡入</br>
•fade_out，淡出</br>
•push_down_in，从下方推入</br>
•push_down_out，从下方推出</br>
•slide_in_from_top，从头部滑动进入</br>
•zoom_enter，变形进入</br>
•shrink_to_middle，中间缩小</br>

* Android基本控件变量命名：</br>
<table class="table table-bordered table-striped table-condensed">
    <tr>
        <td>TextView</td>
        <td>txt_ +描述</td>
        <td>DatePicker</td>
        <td>dtPk_+描述</td>
    </tr>
    <tr>
        <td>Button</td>
        <td>btn_+描述</td>
        <td>TimePicker </td>
        <td>tmPk_+描述</td>
    </tr>
    <tr>
        <td>ImageButton </td>
        <td>imgBtn_+描述</td>
        <td>ToggleButton</td>
        <td>tglBtn_+描述</td>
    </tr>
    <tr>
        <td>ImageView</td>
        <td>img_+描述 </td>
        <td>EditText</td>
        <td>edt_+描述</td>
    </tr>
    <tr>
        <td>CheckBox</td>
        <td>chk_+描述 </td>
        <td>ProgressBar</td>
        <td>progress_+描述</td>
    </tr>
    <tr>
        <td>RadioButton</td>
        <td>rdoBtn_+描述</td>
        <td>SeekBar</td>
        <td>skBar_+描述</td>
    </tr>
    <tr>
        <td>AnalogClock </td>
        <td>anaClk_+描述</td>
        <td>AutoCompleteTextView</td>
        <td>autoTxt_+描述</td>
    </tr>
    <tr>
        <td>ZoomControls</td>
        <td>zmCtrl_+描述</td>
        <td>WebView </td>
        <td>webV_+描述</td>
    </tr>
    <tr>
        <td>Include </td>
        <td>ind_+描述</td>
        <td>RatingBar</td>
        <td>ratBar_+描述</td>
    </tr>
    <tr>
        <td>VideoView</td>
        <td>vdoV_+描述</td>
        <td>Gallery </td>
        <td>gal_+描述</td>
    </tr>
    <tr>
        <td>Tab</td>
        <td>tab__+描述</td>
        <td>ImageSwitcher </td>
        <td>imgSwt_+描述</td>
    </tr>
    <tr>
        <td>Spinner</td>
        <td>spn_+描述</td>
        <td>GridView </td>
        <td>gV_+描述</td>
    </tr>
    <tr>
        <td>ScrollView</td>
        <td>sclV_+描述</td>
        <td>ListView </td>
        <td>listV_+描述</td>
    </tr>
    <tr>
        <td>TextSwitcher </td>
        <td>txtSwt_+描述</td>
        <td>MapView </td>
        <td>mapV_+描述</td>
    </tr>
    <tr>
        <td>Chronometer</td>
        <td>cmt_+描述</td>
        <td>ExpandableList</td>
        <td>epdLt_+描述 </td>
    </tr>
    <tr>
        <td>DigitalClock </td>
        <td>dgtClk_+描述</td>
        <td>MultiAutoCompleteTextView </td>
        <td>mlAutoTxt_+描述</td>
    </tr>
    <tr>
        <td>TableLayout</td>
        <td>table_+描述</td>
        <td>TableRow</td>
        <td>row_+描述</td>
    </tr>
    <tr>
        <td>SearchView</td>
        <td>sechV_+描述</td>
        <td>RadioGroup</td>
        <td>rGroup_描述</td>
    </tr>
    <tr>
        <td>LinearLayout</td>
        <td>llayout_+描述</td>
        <td>RelativeLayout</td>
        <td>rlayout_+描述</td>
    </tr>
    <tr>
        <td>TabHost</td>
        <td>host_描述</td>
        <td>TabWidget</td>
        <td>widget_+描述</td>
    </tr>
</table>

* 程序默认图标 </br>
  若未指定程序图标，均采用默认图标，各规格图标如下：</br>
![40](https://github.com/weiyashuai123/Code-specification/blob/master/icon40.png "40x40")
![80](https://github.com/weiyashuai123/Code-specification/blob/master/icon80.png "80x80")
![120](https://github.com/weiyashuai123/Code-specification/blob/master/icon120.png "120x120")
![240](https://github.com/weiyashuai123/Code-specification/blob/master/icon240.png "240x240")


Create At：2016年9月20日             
Update At：2017年4月8日              
Author：魏亚帅                       
E-mail：subcakewei@outlook.com       
GitHub：github.com/weiyashuai123      

