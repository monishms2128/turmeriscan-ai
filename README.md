# TurmeriScan AI — Hackathon Demo Bundle

This bundle contains the updated Streamlit application and the ten spectral sample images supplied for the judge demonstration.

## Included demo labels

The application treats the first five supplied samples as **Pure** and the next five supplied samples as **Adulterated**, following the labeling provided for this demo. These labels are shown as supplied reference labels for comparison with the model output; they are not recomputed by the application.

## Folder structure

```text
turmeriscan_refined.py
demo_samples/
  pure/
    pure_sample_01.jpg ... pure_sample_05.jpg
  adulterated/
    adulterated_sample_01.jpg ... adulterated_sample_05.jpg
```

Place the trained model file `turmeric_binary_final.h5` beside `turmeriscan_refined.py`.

## Run

Install the dependencies:

```bash
pip install streamlit tensorflow pillow opencv-python-headless numpy pandas
```

Start the app:

```bash
streamlit run turmeriscan_refined.py
```

Use **Run 10-sample judge demo** to screen all packaged spectral images in one click. The results show the model verdict, confidence, supplied reference label, agreement check, enhanced preprocessing preview, and a downloadable CSV summary.

For the presentation, explain that the demo illustrates the complete workflow: spectral image input, preprocessing, CNN prediction, confidence thresholding, and review-oriented output. Keep the laboratory-validation limitation visible during the demo.
