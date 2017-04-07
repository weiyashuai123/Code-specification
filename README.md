# Android自定开发规范</br>
* 基本规范：</br>
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
•文字大小的单位统一用sp，控件大小的单位统一用dp。</br>
•应用中的字符串统一在strings.xml中定义，然后在代码和布局文件中引用。</br>
•颜色值统一在colors.xml中定义，然后在代码和布局文件中引用。（不要用系统的颜色）</br>

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
    <tr>
        <td></td>
    </tr>
</table>
