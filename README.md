# CNN-Visualization-Using-Streamlit
Visualize CNN Classification of Malaria-infected Cells using Streamlit

## Read the Documentation [Here](https://nazillymada.github.io/Classification-of-Malaria-infected-Cells/)

### Running Visualization Using Streamlit on your local environment
**Install Streamlit first**
```
py -m pip install streamlit
```
**Download/Clone this Repository**

**Change some script in cnn-streamlit.py**
```
# Change path of the weights file
@st.cache(allow_output_mutation=True,suppress_st_warning=True)
def load_cnn1():
    model_ = load_model('Change-to-your-path/weights1.h5')
    return model_

@st.cache(allow_output_mutation=True,suppress_st_warning=True)
def load_cnn2():
    model_ = load_model('Change-to-your-path/weights3.h5')
    return model_

# Change path of sample file
 
 elif choice== 2 :
        st.subheader("Sample Data")
        sample1 = Image.open('Change-to-your-path/Capture.png')
        st.image(sample1,caption='Parasitized Cells', use_column_width=True)
        sample2 = Image.open('Change-to-your-path/Capture1.png')
        st.image(sample2,caption='Uninfected Cells', use_column_width=True)
        st.markdown("#### Training and Testing Sets")
        """
```

**Run the script**
Run this script in terminal/command prompt
```
streamlit run cnn-streamlit.py
```
