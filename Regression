import pickle
import streamlit as st

WS_Predictor = pickle.load(open ('PrediksiWS.sav'))

st.title ('WS Predictor')

RPM_Feeder = st.text_input ('Masukkan Nilai RPM Feeder')
AMP_Press = st.text_input ('Masukkan Nilai Ampere Mesin Press')
Temp_Cond_1 = st.text_input ('Masukkan Nilai Temp Cond 1')
Temp_Cond_2 = st.text_input ('Masukkan Nilai Temp Cond 2')
Temp_Cond_3 = st.text_input ('Masukkan Nilai Temp Cond 3')
Temp_Post_Pellet = st.text_input ('Masukkan Nilai Temp Post Pellet')

prediksi = ''

if st.button('Prediksi WS'):
    prediksi = model.predict(
        [['RPM_Feeder, Amp_Press, Temp_Cond_1, Temp_Cond_2, Temp_Cond_3, Temp_Post_Pellet']]
    )
    st.write ('Ketinggian enfapan WS diprediksi sekitar : ', prediksi)