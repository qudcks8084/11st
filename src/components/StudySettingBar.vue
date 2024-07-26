<template>
    <div id="StudySettingBar">
      <span id="SettingBarSetting">학습 방법</span>
      <span>|</span>
      <select id="CodeGroupSetting">
        <option value="따라치기">따라치기</option>
        <option value="줄별 순서맞추기">줄별 순서맞추기</option>
        <option value="블록 순서맞추기">블록 순서맞추기</option>
        <option value="빈칸 채우기">빈칸 채우기</option>
      </select>
      <span id="SettingBarSetting">난이도</span>
      <span>|</span>
      <select name="LevelSetting" id="CodeGroupSetting">
        <option value="1">1 레벨</option>
        <option value="2">2 레벨</option>
        <option value="3">3 레벨</option>
      </select>
      <span id="SettingBarSetting">코드 그룹</span>
      <span>|</span>
      <select name="CodeGroupSetting" id="CodeGroupSetting">
        <option value='{"id": -1, "name": "Default", "language": "Default", "owner": {"id": 0, "name": "Default"}}'>선택 안됨</option>
        <option value='{"id": 1, "name": "Example Group", "language": "JavaScript", "owner": {"id": 1, "name": "Example Owner"}}'>Example Group / JavaScript / Example Owner</option>
        <!-- Add more options here as needed -->
      </select>
      <button id="ProblemSettingIcon">
        <span>문제 출제하기</span>
      </button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'StudySettingBar'
  };
  </script>
  
  <style scoped>
  #StudySettingBar {
    width: 85%;
    height: 3vh;
    margin-top: 7.5vh;    
    margin-left: 7.5vw;
    margin-right: 7.5vw;
    display: grid;
    grid-template-columns: 1fr 0.5fr 1fr 0.75fr 0.5fr 0.75fr 1fr 0.5fr 3.5fr 2fr ;
    justify-items: center;
    align-items: center;
    font-size: medium;
  }
  
  #SettingBarSetting {
    font-weight: bold;
  }
  
  #CodeGroupSetting {
    border: 0px;
    font-family: 'SUITE-Regular';
    font-size: medium;
  }
  
  #ProblemSettingIcon {
    width: 10vw;
    height: 3vh;
    display: flex;
    justify-content: center;
    align-items: center;
    border: 1px solid #ddd;
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    background-color: #fff;
    transition: box-shadow 0.3s ease;
  }
  
  #ProblemSettingIcon:hover {
    box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
  }
  
  #CodeGroupSettingList {
    font-family: 'SUITE-Regular';
    background-color: white;
  }
  </style>
  