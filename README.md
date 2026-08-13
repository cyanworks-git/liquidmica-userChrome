<div align="center">
<img width="500" height="333" alt="index" src="https://github.com/user-attachments/assets/68c90e88-03c6-4d31-a0c2-4dde1501ba78" />
  <div id="user-content-toc">
    <ul align="center" style="list-style: none; padding: 0; margin: 0;">
      <summary>
        <h1>Liquid Mica</h1>
      </summary>
      <img src="https://img.shields.io/badge/Firefox-153.0.3-FF7139?style=flat&logo=firefoxbrowser&logoColor=white"/>
      <img src="https://img.shields.io/badge/Firefox Developer Edition-154.0b10-0093EE?style=flat&logo=firefoxbrowser&logoColor=white"/>
      <img src="https://img.shields.io/badge/Floorp-12.16.4@153.0-5309E8?style=flat&logo=floorp&logoColor=white"/>
    </ul>
    
   </div>
   
MacOS의 리퀴드 글래스 느낌을 Windows의 Mica와 혼합한 FireFox userChrome 테마.

[Read in English](./README.en.md)

</div>

## 개요
이 테마는 기존의 밋밋한 FireFox 창에서 벗어나 MacOS의 리퀴드 글래스 느낌을 주면 어떨까 하여 ChatGPT(codex) 바이브 코딩으로 제작한 테마입니다(+Gemini 도움도 받음).

메뉴창, 메시지 상자, 알림 팝업 등 최대한 스타일에 맞게 수정되었으며, 밋밋한 메뉴창에 일부 아이콘을 추가하고 세로 탭에서도 테마가 유연하게 적용되도록 만들었습니다.

## 미리보기
<details>
  <summary>펼쳐서 미리보기</summary>
  <img width="1431" height="932" alt="1" src="https://github.com/user-attachments/assets/a843df25-fc12-4164-ac81-bec0c87c7804" />
  <img width="1431" height="932" alt="2" src="https://github.com/user-attachments/assets/b6ad72f8-6cba-4034-9259-98e6a09e0b6b" />
  <img width="1431" height="932" alt="3" src="https://github.com/user-attachments/assets/00dc6a1d-3c03-4638-9b88-5654fc79b7fb" />
  <img width="1431" height="932" alt="4" src="https://github.com/user-attachments/assets/66f22a22-51f2-4c77-94c9-0d8c69b4ac18" />
  <img width="1431" height="932" alt="5" src="https://github.com/user-attachments/assets/464ee584-a0f5-405f-a4fa-a3fd2d9cbe2d" />
</details>

## 설치 방법
> [!WARNING]
> * 본 테마는 Windows 11 다크 모드에서 테스트되었습니다. 라이트 모드에서는 지원되지 않습니다.
> * Windows의 Mica 디자인 시스템이 적용되기 때문에 다른 운영체제에서는 호환되지 않습니다.
> * 본 테마는 <b>Firefox 153.0.3</b>, <b>Firefox Developer Edition 154.0b10</b>  및 <b>Floorp 12.16.4@153.0</b>에서 테스트되었습니다. 이전 버전에서 사용시 테마 스타일이 깨질 수 있습니다.
### 설치 전 조치사항
1. FireFox 주소에 `about:config`를 입력합니다. 경고 화면이 뜰 경우 `위험을 감수하고 계속`을 누릅니다.
2. `toolkit.legacyUserProfileCustomizations.stylesheets`를 찾아 더블 클릭으로 `true`로 만듭니다.
3. `widget.windows.mica`를 찾아 더블 클릭으로 `true`로 만듭니다.
4. `widget.windows.mica.popups`를 찾아 `1` 혹은 `2`로 기본 설정되어 있는지 확인합니다. `0`으로 되어있을 경우 더블 클릭으로 불린 값을 해당 값으로 조정합니다.
5. `widget.windows.mica.toplevel-backdrop`을 찾아 더블 클릭으로 불린 값을 `2`로 조정합니다.
### 설치 및 적용방법 
1. 페이지 상단에 `Code` → `Download ZIP`을 눌러 압축파일로 저장합니다.
2. FireFox 주소에 `about:profiles`를 입력합니다.
3. 사용 중인 프로필의 루트 디렉터리의 `폴더 열기`를 누릅니다.
4. `Chrome` 폴더를 생성하여 그 폴더에서 내려받은 파일들을 이동합니다.
5. `liquidmica.css`를 `userChrome.css`로 이름을 변경하거나 해당 이름으로 css 파일 생성 후 다음과 같이 수정하여 저장합니다:
   <br><br>
   ```css
   @import url("liquidmica.css");
   ```
6. FireFox를 재시작 합니다.
<br>
<br>


<img width="100%" alt="6" src="https://github.com/user-attachments/assets/ed065261-dd11-450f-94e1-e5cc1d128cb6" />

## Floorp 대응
이 테마는 같은 Gecko(FireFox) 기반인 Floorp 브라우저에도 이용할 수 있도록 대응하였습니다. 이는 `liquidmica_for_floorp.css`가 그 역할을 합니다.

기존 Floorp와 다르게 전용 사이드바는 왼족으로 고정되며(현재 Floorp Hub로 방향 설정 불가), 세로 탭 혹은 FireFox 기본 사이드바가 왼쪽에 켜져있을 때 Floorp 사이드바는 오른쪽으로 배치되게끔 하여 배치 순서를 바꿨습니다. 패널 또한 바로 옆에 올바르게 배치됩니다.

또한, Floorp 관련 메뉴들과 창 역시 본 테마에 맞게 적용되었습니다.
### Floorp에서 테마 저장 방법
> [!NOTE]
> 테마를 올바르게 적용하려면 반드시 `Proton` 테마를 사용해야 합니다.
> 이는 `메뉴(☰)` → `Floorp Hub`(현 버전에서는 번역 오류로 빈 칸으로 되어 있습니다) → 설정 페이지의 `탭 및 모양`에서 설정하실 수 있습니다.
1. 페이지 상단에 `Code` → `Download ZIP`을 눌러 압축파일로 저장합니다.
2. Floorp에서 `메뉴(☰)`를 누르고 `스타일` → `스타일 시트 폴더 열기`를 누르면 설치할 chrome 경로로 이동합니다.
3. 내려받았던 파일을 해당 폴더에서 저장합니다.
4. Floorp를 재시작하여 적용되어 있는지 확인합니다.
> [!TIP]
> * `메뉴(☰)` → `스타일`에서 css 파일 4개가 정상적으로 보여야 합니다.
> * `✓ liquidmica.css`만 되어 있어도 모든 스타일이 정상적으로 적용됩니다.
