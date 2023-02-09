import pandas_profiling import ProfileReport
# Se a parada não funcionar: !pip install https://github.com/pandas-profiling/pandas-profiling/archive/master.zip
profile = ProfileReport(df, title="Pandas Profilling Report", html={"style":{"full_width": True}})
profile
