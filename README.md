# ToDo_List_Class 

Start React 2021.01.11

EMRO 컨버전 개발팁
================================================================================================================
$logger.info("resultMap ====>"+resultMap);
initialized
isEmpty
formulas
{{formula('test')}}
window.close();
<div class="hspace-2"></div>
<div class="field-box">
SCLoadMask.show();
isSelectionChecked    << 체크여부
translate
<sc-trigger-field trigger-cls="search" on-click="popupModuleShop"></sc-trigger-field>
observers : []
mask-re
value-field
display-field
colspan="4"
<div class="flex page">
	<div class="vbox fit">
		class="vbox flex-5"
		class="flex"
	</div>
</div>
class="align-right"
search-button-hidden="true"

event.target.id   ->  event.currentTarget.id

UT.formatDate(toDay,'yyyyMMdd')

CCContentBase  -> ESCommConst


<sc-period-date-field from-value="{{_shopPurchaseRequestReceiptSearchParameter.pr_req_date_fr}}" 
                      to-value="{{_shopPurchaseRequestReceiptSearchParameter.pr_req_date_to}}"
    										default-from-value="-1M" default-to-value="0d"	
   											string-date="true">
    								</sc-period-date-field>


<sc-link rel="import" href="../org/ep-dept-tree-pop.html"></sc-link>

UT.isEmpty()

            	var data = event.detail.data;
            	var item = event.detail.item;
            	var provider = event.detail.provider;
            	var datafield = item.dataField;

                    	var rowIndex = event.detail.item.rowIndex;
                    	var newValue = event.detail.newValue;
                    	var oldValue = event.detail.oldValue;

	SCSessionManager.getCurrentUser()


                var defaultParam = {
                    oper_org_sn : me.get("headerSO.oper_org_sn"),
                    itemList    : allItems,
                    rfx_flag    : "X",
                    ext_cd      : "002",
                    isMultiple  : true,
	        mode : ESCommConst.VIEW
                };
            	var ePShopPopup = UT.popup('ep-shop', me, 700, 400, {
            		"selected-item" : function(popup, e) {
            			var receiver = e.detail;
            			me.set('_shopPurchaseRequestReceiptSearchParameter.shop_cd',receiver["shop_cd"]);
            			me.set('_shopPurchaseRequestReceiptSearchParameter.shop_nm',receiver["shop_nm"]);
            			popup.close();
            		},
            		"close" : function(popup, e) {
            			popup.close();
            		},
            	},{
            		title : '업장현황'
            	});
            	ePShopPopup.show();
            	ePShopPopup.getWindowContent().load(sender);



            formulas: {
            	_showAprvStatus: function(){
            		return this._showAprvStatus;
            	},
            },


	this.applyFormula();


	{{!formula('isUseSelection')}}


	UT.makeConsoleLogGridFields(resultList[0], this.$.datagrid, null);

                __codes: {
                    type: Object,
                    value: function() {
                        return {
                        	D002 : [],
                        	D003 : []
                        };
                    }
                }

	가로구분선 -----
	<sc-splitter split-type="horizontal"></sc-splitter>
	세로구분선 |||||
	<sc-splitter split-type="vertical"></sc-splitter>

	show-selection-header="false"


	qty -> decimal    1.0000 -> 1.00
	wgt -> decimal
	amt -> integer

    var provider   = me.$.pagingDatagrid.getDataProvider();
    var selectItem = provider.selectionCheckedItems();
		var unSelecItem = provider.selectionUnCheckedItems();
		var allItems = provider.getItems();
		var updateItems = provider.getUpdateItems();
		var newItems = provider.getNewItems();
		var removeItems = provider.getRemoveItems();
		var indexArr =  provider.selectionCheckedIndexes();
		var indexes = provider.selectionUnCheckedIndexes();

	input-clear="false"
	selected-index="0"

	// 그리드 체크박스 체크
	me.$.purRqItemGrid.selectionCheck(i,true,false);

	// 그리드 sort
	,{visibleOnly:true});

	this.translate();

	validation-group="saveValidator"
	this.validate('requiredValidator')



								provider.removeItemAtBatch(deleteIndexArr, function(index, data){
									if(data.newitem == "true"){
										return true; 
									}
								});


	                            provider.setItemAtBatch(me.rowIndex, function(index, data){
	                            	return itemRow;
								},{visibleOnly:true});

				},{visibleOnly:true});

<sc-trigger-field trigger-cls="search" on-click="callModuleForm" auth-editicon text="wh_cd"></sc-trigger-field>


cc-sub-title-bar

                            UT.getAprvInfo(me, aprvInfo, function(e){
                            	var result = e.detail.result;
                            });



editor-maskre   ->    mask-re

 /  -> <span style="margin:0 5px">&#47;</span>
  <span style="margin-left:5px">[[translate('차')]]</span>
<sc-label text="분" style="margin:0 2px"></sc-label>

// 숫자 오른쪽정렬
text-align: right;
input-cover="true"
class="align-right w-120"

// 대용량조회
large="true" target="{{_extendTargList}}"

<sc-period-date-field from-value="{{_searchParam.pr_req_date_fr}}" 
                      to-value="{{_searchParam.pr_req_date_to}}"
                      default-from-value="-7d"
                      default-to-value="0d" 
  										string-date="true">
</sc-period-date-field>

<img src="/ui/assets/img/grid/icon_link.png" alt="" hidden="{{!chr_reason}}" on-click="chr_reason_click"></img>

// 그리드 체크박스 , 라디오버튼 클릭제어
on-selection-checked="onSelectionChecked"
editor-regex="/^[-0123456789]+([.]?[0-9]{0,2})$/"

================================================================================================================


기이드
http://techdocs.emro.co.kr/display/SF9/grid+dataProvider
http://175.124.141.220/devops.do - 구축
http://175.124.141.220/docs.do 
http://techdocs.emro.co.kr/display/SF9/Intro 
http://helpme.emro.co.kr/projects/grid/api/ko/Examples 

***********************************************************************************
****** 태그 ******
***********************************************************************************
<cc-search-container hide-buttons="true" //검색 버튼 숨김
테이블 그룹단위 validation
validation-group="searchValid"
태그 required="true"인 필드에 적용

data-provider => items
data-field => value-field
label-field => display-field
validate-on-cell-paste="true" => 삭제
editor-maskre => mask-re
mask-re="/[a-zA-Z0-9]/" 
upper-case="true" 
strip-chars-re="/[ㄱ-힣]/"
//팝업호출하여 리턴된 값이 라벨에 넣어줄때
on-click => on-trigger-click
style="width:120px;"
<cc-page-title-bar title-text="{{menuName}}">
placeholder="전체"
input-clear="false" //콤보박스 
selected-index="0" // 콤보박스 

//달력
<sc-period-date-field from-value="{{searchSO.from_date}}"
                             to-value="{{searchSO.to_date}}"
                             string-date="true"
</sc-period-date-field>

<cc-date-field id="slip_dt"> => <sc-date-field value="{{searchSO.slip_dt}}">

<div id = "soptVendor" => 숨김 처리
<to-be>
me.$.soptVendor.hidden = true;
<as-is>
me.$.soptVendor.__setter__visible(false);
me.$.soptVendor.includeInLayout = false;

가로구분선 -----
<sc-splitter split-type="horizontal"></sc-splitter>
세로구분선 |||||
<sc-splitter split-type="vertical"></sc-splitter>

** 그리드 **
show-number-line="false" //그리드 열에 대한 번호

//그리드 필드 추가 
var es = document.querySelector('ep-claim-item-list-popup');
var grid = es.$.datagrid;
var list = grid.getDataProvider().getItems();
UT.makeConsoleLogGridFields(list[0], grid, null); 

***********************************************************************************
*** 스크립트 ****
***********************************************************************************
//초기화 함수
initialized
observers : []
event.target  검색->  this.$.searchSP
event.target.id(event.currentTarget.id)   검색->  "searchSP"
//set => add 변경
setInput => addInput
valueCopy => UT.copy
//멀티콤보박스의 빈 값을 넘길때 
param.wh_cntr_cd = UT.isEmpty(param.wh_cntr_cd) ? "''" : "'" + param.wh_cntr_cd.join("','") + "'";
// 세션정보 : session
SCSessionManager.getCurrentUser();
// 그리드 체크박스 체크
me.$.그리드아이디.selectionCheck(i,true,false);
for(var i = 0; i < length; i++){
       grid.selectionCheck(checkedIndexes[i], false, true);
}

<script> properties에서 아래 코드유무 확인 후 없으면 추가 
                __codes: {
                    type: Object,
                    value: function() {
                        return {
                        	C102 : [],
                        	D003 : []
                        };
                    }
                }
** 엑셀 대용량 업로드 **
<cc-excel-export
	id="exporter"
	params="{{_claimSearchParam}}"
	service-fn="stats,get.claimresult.exc`eldown">
</cc-excel-export>

** 달력 **
var now = new Date();
this.set("_claimSearchParam.fromdt", UT.formatDate(now,'yyyyMMdd'));
this.set("_claimSearchParam.todt", UT.formatDate(now,'yyyyMMdd'));

**** 그리드 셀렉트 체크/해제 ***
<sc-checkbox-column>  주석처리

var rowIndex = event.detail.item.rowIndex; // 선택한 그리드의 row


//그리드 데이터 호출
           	var provider   = me.$.datagrid.getDataProvider(); 
            	var selectItem = provider.selectionCheckedItems(); //선택한 아이템
	var unSelecItem = provider.selectionUnCheckedItems(); // 선택안한 아이템
	var allItems = provider.getItems(); //모든 아이템
	var updateItems = provider.getUpdateItems(); 
	var newItems = provider.getNewItems();
	var removeItems = provider.getRemoveItems();
	var indexArr =  provider.selectionCheckedIndexes(); //index 배열
	var indexes = provider.selectionUnCheckedIndexes(); //

// 그리드에서 선택한 row에 데이터 변경
 provider.setItemAtBatch([me.get("rowIndex")], function(indexSub, dataSub){
    	return nowdata;
 },{visibleOnly:true});

두가지 사용법
/*     nowitem.movement_typ = popupitem.dtl_cd;
       nowitem.movement_typ_nm = popupitem.dtl_cd_nm; */
 provider.setItemAtBatch([me.get("rowIndex")], function(indexSub, dataSub){
             dataSub.movement_typ = popupitem.dtl_cd;
             dataSub.movement_typ_nm = popupitem.dtl_cd_nm;
             return dataSub;
},{visibleOnly:true});

  nowitem.movement_typ = popupitem.dtl_cd;
  nowitem.movement_typ_nm = popupitem.dtl_cd_nm; 
 provider.setItemAtBatch([me.get("rowIndex")], function(indexSub, dataSub){
        return nowitem;
},{visibleOnly:true});


//그리드에서 아이템 클릭
            	var data = event.detail.data;
            	var item = event.detail.item;
            	var provider = event.detail.provider;
            	var datafield = item.dataField;
             var rowIndex = event.detail.item.rowIndex;
             var newValue = event.detail.newValue;
             var oldValue = event.detail.oldValue;

//라벨 클리어 함수
commonPopupValueClear: function(event) {
            	var me = this;
            	var id = event.currentTarget.id;
            	switch (id) {
	                case "jrnl_typ_cd":
	                	me.set("searchSO.jrnl_typ_nm", "");
	                    break;
	                default:
	                    break;
	            }
            }, 


formatters.js -> 포멧

// 콤보박스 removeAll
this.$.아이디.items = [];


mu_cd

resultHandler 
var check = false; 
for(var i in this.buCdList){ 
if(this.buCdList[i].data == SCSessionManager.getCurrentUser().s_bu_cd) check = true; 
} 
if(check == false) this.set("searchSO.bu_cd", ''); 
check = false; 
for(var i in this.mucdlist){ 
if(this.mucdlist[i].data == SCSessionManager.getCurrentUser().s_mu_cd) check = true; 
} 
if(check == false) this.set("searchSO.mu_cd", '');  


UT.alertShow(me.translate("업체 '{0}'의 발행구분이 없습니다. 업체정보에서 발행구분을 입력하세요.", me, [item.vd_nm]));



<div class="field-box">
                                <sc-text-field id="dept_cd" 
                                               name="code" 
                                               style="width:80px;" 
                                               readonly="true" 
                                               required="true" 
                                               on-enter="popupModuleForm" 
                                               on-change="commonPopupValueClear" 
                                               value="{{searchSO.dept_cd}}">
                                </sc-text-field>
                                <div class="hspace-2"></div>
                                <sc-trigger-field trigger-cls="search" on-click="popupModuleForm"></sc-trigger-field>
                                <div class="hspace-2"></div>
                                <!--CONVERTER (ELEMENT 삭제) : <vc:SCButton id="dept_cd_btn" styleName="linkIcon" click="popupModuleForm(event)"></vc:SCButton>-->
                                <sc-label id="dept_nm" name="name" text="{{searchSO.dept_nm}}"></sc-label>
                            </div>




// readonly="true" 인경우 버튼 안보이면 새로 버튼 만들어준다
<div class="hspace-2"></div>
                                
<sc-trigger-field trigger-cls="search" on-click="popupModuleForm"></sc-trigger-field>
                                
<div class="hspace-2"></div>


//정산담당자 팝업 초기세팅
usr_id 값
sender.defaultParam = {usr_id : me.$.acc_chr_id.value};


//그리드 합계 두칸
aggregate-title="합계" aggregate-footer-span-next="1" aggregate-text-align="center"

//더하기
aggregate-kind="sum" aggregate-format="number" data-type="number" 


// ExternalInterface.call 변환
변경전
ExternalInterface.call('getAprvInfo', aprvInfo); 
변경후
UT.getAprvInfo(this, aprvInfo, null);


//리포트 호출함수
UT.reportViewer(reportParameter, 1);

//로컬에서 결재요청 테스트를 위한 코드
TestSloCreate.java 
public static String empNo = ""; 
    public static void setEmpNo(String usrId) {
    	empNo = usrId;
    }  


//결재후 부모 창으로 돌아가기
 doAprv: function() {
aprvInfo.owner = "em-sh-cost-slip-sts";
}



//그리드 아이템에 클릭 있는경우
<sc-grid  on-item-click="clickFunc">
<sc-grid-columns>
<cc-popup-icon-column> => <sc-data-column> 변경
click="clickFunc" 삭제 후 on-item-click 추가
</sc-grid-columns>
</sc-grid>



                __codes: {
                    type: Object,
                    value: function() {
                        return {
                        	P045 : [],
                        	C102 : []
                        };
                    }
                },

// 달력 기간

<sc-period-date-field from-value="{{searchSO.from_date}}"
                                                              to-value="{{searchSO.to_date}}"
                                                              string-date="true"
                                                              required="true" style="width:200px">
                                        </sc-period-date-field>


//콤보박스 하드코딩

close_typ: {
                    type : Array,
                    value : function(){
                        return [
                                {data : "GR", label : "매입"},
                                {data : "GI", label : "원가"},
                                {data : "MV", label : "이동"}
                                ];
                    }
                },

$logger.info()


$service.callJob("interface.sap.003.budget.assign");

id="get.sh.buy.close.list" label="매입마감 조회"


http://gitlab.emro.co.kr/ 
emrouser
emro1004!



================================================================================================================
  
  
  
popup-module-properties.html => 팝업리스트


*******************
****** 태그 ******
*******************
data-provider => items
editor-maskre => mask-re
data-field => value-field
label-field => display-field
on-trigger-click
style="width:120px;"
mask-re="/[a-zA-Z0-9]/" 
upper-case="true" 
strip-chars-re="/[ㄱ-힣]/"
title-text =""
placeholder="전체"
show-number-line="false" //그리드 행
validate-on-cell-paste="true" 삭제
input-clear="false" //콤보박스 
selected-index="0" // 콤보박스 
hide-buttons="true" //검색 버튼 숨김

sc-grid-columns 아래에 sc-grid-fields, sc-grid-field 추가 해야함
스크립트 itemClickHandler 함수 실행 시 아래 구문 추가
UT.makeConsoleLogGridFields(this._claimResultList[0], this.$.datagrid, null); 

data-field=" check_select " 인 경우 와 data-field=" check_delet " 인 경우 <sc-checkbox-column 주석처리 후 
<sc-grid 의 use-selection="true" 변경

//달력
                                <sc-period-date-field from-value="{{}}"
                                                      to-value="{{}}"
                                                      string-date="true"
                                                      required="true"
                                                      default-from-value="-1M"
                                                      default-to-value="0d">
                                </sc-period-date-field>

//안쓰이는 코드
validate-on-cell-paste="true"
<sc-panel collapsible="true">

	가로구분선 -----
	<sc-splitter split-type="horizontal"></sc-splitter>
	세로구분선 |||||
	<sc-splitter split-type="vertical"></sc-splitter>


<cc-date-field id="slip_dt"> => <sc-date-field value="{{searchSO.slip_dt}}">

<div id = "soptVendor"
me.$.soptVendor.hidden = true;
아래코드와 같다
me.$.soptVendor.__setter__visible(false);
me.$.soptVendor.includeInLayout = false;


***********************************************************************************
*** 스크립트 ****
*******************

observers : []
event.target.id   ->  event.currentTarget.id
setInput => addInput
valueCopy => UT.copy
UT.multiComboboxChange(this.$.변수명.value); // 쿼리 조회시 배열 {}문자 정리
SCSessionManager.getCurrentUser() // 세션정보 : session
initialized

// 그리드 체크박스 체크
me.$.purRqItemGrid.selectionCheck(i,true,false);
// 그리드 sort,{visibleOnly:true});

//데이터 초기화 시 
sc-service-group 태그에 값이 안보이는 경우 
<script> properties에서 아래 코드유무 확인 후 없으면 추가 
                __codes: {
                    type: Object,
                    value: function() {
                        return {
                        	C102 : [],
                        	D003 : []
                        };
                    }
                }

// 히든태그 추가 
var es = document.querySelector('ep-claim-item-list-popup');
var grid = es.$.datagrid;
var list = grid.getDataProvider().getItems();
UT.makeConsoleLogGridFields(list[0], grid, null); 


** 엑셀 대용량 업로드 **
<cc-excel-export
	id="exporter"
	params="{{_claimSearchParam}}"
	service-fn="stats,get.claimresult.exc`eldown">
</cc-excel-export>


** 달력 **
var now = new Date();
this.set("_claimSearchParam.fromdt", UT.formatDate(now,'yyyyMMdd'));
this.set("_claimSearchParam.todt", UT.formatDate(now,'yyyyMMdd'));



** 팝업 찾기 ***
SP001 => ep-sp001.html


**** 그리드 셀렉트 체크/해제 ***
<sc-checkbox-column>  주석처리

var rowIndex = event.detail.item.rowIndex; // 선택한 그리드의 row


//그리드 데이터 호출
           	var provider   = me.$.datagrid.getDataProvider(); 
            	var selectItem = provider.selectionCheckedItems(); //선택한 아이템
		var unSelecItem = provider.selectionUnCheckedItems(); // 선택안한 아이템
		var allItems = provider.getItems(); //모든 아이템
		var updateItems = provider.getUpdateItems(); 
		var newItems = provider.getNewItems();
		var removeItems = provider.getRemoveItems();
		var indexArr =  provider.selectionCheckedIndexes(); //index 배열
		var indexes = provider.selectionUnCheckedIndexes(); //

// 그리드에서 선택한 row에 데이터 변경
 provider.setItemAtBatch([me.get("rowIndex")], function(indexSub, dataSub){
    	return nowdata;
 },{visibleOnly:true});

두가지 사용법
/*     nowitem.movement_typ = popupitem.dtl_cd;
       nowitem.movement_typ_nm = popupitem.dtl_cd_nm; */
 provider.setItemAtBatch([me.get("rowIndex")], function(indexSub, dataSub){
             dataSub.movement_typ = popupitem.dtl_cd;
             dataSub.movement_typ_nm = popupitem.dtl_cd_nm;
             return dataSub;
},{visibleOnly:true});

  nowitem.movement_typ = popupitem.dtl_cd;
  nowitem.movement_typ_nm = popupitem.dtl_cd_nm; 
 provider.setItemAtBatch([me.get("rowIndex")], function(indexSub, dataSub){
        return nowitem;
},{visibleOnly:true});


//그리드에서 아이템 클릭
            	var data = event.detail.data;
            	var item = event.detail.item;
            	var provider = event.detail.provider;
            	var datafield = item.dataField;

                    	var rowIndex = event.detail.item.rowIndex;
                    	var newValue = event.detail.newValue;
                    	var oldValue = event.detail.oldValue;




//라벨 클리어 함수
commonPopupValueClear: function(event) {
            	var me = this;
            	var id = event.currentTarget.id;
            	switch (id) {
	                case "jrnl_typ_cd":
	                	me.set("searchSO.jrnl_typ_nm", "");
	                    break;
	                default:
	                    break;
	            }
            }, 
//null 체크
UT.isEmpty();


//그리드 체크박스 예제
ES-SG-USER-LIST



//set 
this.set("rowIndex",rowIndex);
//get
this.get("rowIndex",rowIndex);
// function 안에 function 에서 this 사용 x -> var me = this 사용

/*소스명*/
formatters.js -> 포멧


var id = event.currentTarget.id; // 클릭하는 순간 속성 id
var me = this;
me.$.아이디.value => this에서 가져오는 아이디 value
me.$.아이디.text=> this에서 가져오는 아이디 text

//필드 값 가져오기 
me.searchSO.shop_cd 
me.$.shop_cd.value
위에 두 코드의 결과는 같다

observers : [
'hfcChrPopupValueClear(_claimSearchParam.hfc_chr_id)',
]

// 콤보박스 removeAll
this.$.아이디.items = [];


mu_cd

resultHandler 
var check = false; 
for(var i in this.buCdList){ 
if(this.buCdList[i].data == SCSessionManager.getCurrentUser().s_bu_cd) check = true; 
} 
if(check == false) this.set("searchSO.bu_cd", ''); 
check = false; 
for(var i in this.mucdlist){ 
if(this.mucdlist[i].data == SCSessionManager.getCurrentUser().s_mu_cd) check = true; 
} 
if(check == false) this.set("searchSO.mu_cd", '');  


UT.alertShow(me.translate("업체 '{0}'의 발행구분이 없습니다. 업체정보에서 발행구분을 입력하세요.", me, [item.vd_nm]));



<div class="field-box">
                                <sc-text-field id="dept_cd" 
                                               name="code" 
                                               style="width:80px;" 
                                               readonly="true" 
                                               required="true" 
                                               on-enter="popupModuleForm" 
                                               on-change="commonPopupValueClear" 
                                               value="{{searchSO.dept_cd}}">
                                </sc-text-field>
                                <div class="hspace-2"></div>
                                <sc-trigger-field trigger-cls="search" on-click="popupModuleForm"></sc-trigger-field>
                                <div class="hspace-2"></div>
                                <!--CONVERTER (ELEMENT 삭제) : <vc:SCButton id="dept_cd_btn" styleName="linkIcon" click="popupModuleForm(event)"></vc:SCButton>-->
                                <sc-label id="dept_nm" name="name" text="{{searchSO.dept_nm}}"></sc-label>
                            </div>




// readonly="true" 인경우 버튼 안보이면 새로 버튼 만들어준다
<div class="hspace-2"></div>
                                
<sc-trigger-field trigger-cls="search" on-click="popupModuleForm"></sc-trigger-field>
                                
<div class="hspace-2"></div>


//정산담당자 팝업 초기세팅
usr_id 값
sender.defaultParam = {usr_id : me.$.acc_chr_id.value};


//그리드 합계 두칸
aggregate-title="합계" aggregate-footer-span-next="1" aggregate-text-align="center"

//더하기
aggregate-kind="sum" aggregate-format="number" data-type="number" 


// ExternalInterface.call 변환
변경전
ExternalInterface.call('getAprvInfo', aprvInfo); 
변경후
UT.getAprvInfo(this, aprvInfo, null);


//리포트 호출함수
UT.reportViewer(reportParameter, 1);

//로컬에서 결재요청 테스트를 위한 코드
TestSloCreate.java 
public static String empNo = ""; 
    public static void setEmpNo(String usrId) {
    	empNo = usrId;
    }  


//결재후 부모 창으로 돌아가기
 doAprv: function() {
aprvInfo.owner = "em-sh-cost-slip-sts";
}



//그리드 아이템에 클릭 있는경우
<sc-grid  on-item-click="clickFunc">
<sc-grid-columns>
<cc-popup-icon-column> => <sc-data-column> 변경
click="clickFunc" 삭제 후 on-item-click 추가
</sc-grid-columns>
</sc-grid>



                __codes: {
                    type: Object,
                    value: function() {
                        return {
                        	P045 : [],
                        	C102 : []
                        };
                    }
                },

// 달력 기간

<sc-period-date-field from-value="{{searchSO.from_date}}"
                                                              to-value="{{searchSO.to_date}}"
                                                              string-date="true"
                                                              required="true" style="width:200px">
                                        </sc-period-date-field>


//콤보박스 하드코딩

close_typ: {
                    type : Array,
                    value : function(){
                        return [
                                {data : "GR", label : "매입"},
                                {data : "GI", label : "원가"},
                                {data : "MV", label : "이동"}
                                ];
                    }
                },


$logger.info()


$service.callJob("interface.sap.003.budget.assign");

id="get.sh.buy.close.list" label="매입마감 조회"



http://gitlab.emro.co.kr/ 
emrouser
emro1004!








