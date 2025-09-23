import streamlit as st

st.title('나의 웹 처음 만들기')

name = st.text_input('이름을 입력하세요 : ')
app = st.selectbox('가장 많이 쓰는 앱은?')
time = st.slider('사용 시간은?',0,12,3)
if st.button('나의 디지털 습관은?') :
    st.write(f'{name}님은 {time}시간 동안 {app}st을 많이 사용합니다.')
