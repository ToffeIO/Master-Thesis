## Code
There are two notebooks. DataCleaningAndExploration is a semi-cleaned-up version of what was used during the data exploration phase. Some code blocks have been removed, either because they were not part of the final thesis or for other arbitrary reasons.
ModelsPipeline includes the code used for modelling and plotting results. The code blocks have had their outputs cleaned, yet more code blocks have been removed than remain from the original project.
Below is the introduction and problem formulation of the thesis, which can be seen as the origin of the notebooks' structure.

## Motivation.
Proteomics is a branch of molecular biology that focuses on the large-scale study of
proteins; its components, structure, identification and quantification. The study of
proteomics enables the understanding of how proteins interact with each other, how
their levels change during disease progression and how they contribute to various
biological processes. The advancements of mass spectrometry, a widely used
technique in large-scale proteomics, have revolutionized the field, allowing for rapid
quantification of tens of thousands of peptides and proteins from multiple samples
simultaneously. Furthermore, this advancement has increased the influence of
machine learning (ML) in the field, as more high-dimensional data of larger scale
than before is being produced. Utilizing ML in order to establish disease-associated
proteins for diagnosis, staging, prognosis and treatment is becoming common practice
in proteomic biomarker discovery.

Ideal biomarkers are characterized by their high specificity towards specific disease
conditions. Many biomarkers are proteins expressed in many different diseases,
though their expression levels vary among these diseases. By combining multiple
biomarkers together, it is possible to identify the characteristics and pathogenesis of
individual diseases. One such disease is Alzheimer’s Disease, a neurodegenerative
disorder and the most common form of dementia.

The conventional method for diagnosing AD is through medical history, cognitive tests
and neurological examinations, resulting in a clinical diagnosis. However, a definitive
diagnosis of AD can only be made with certainty through a brain tissue biopsy, known
as a pathological diagnosis. Biomarkers used to give a pathological diagnosis
of Alzheimer’s disease include beta-amyloid protein clumps, known as amyloid
plaques, and neurofibrillary tangles—abnormal tau protein aggregates found in nerve
cells. As these biomarkers can only be found through invasive surgery in the brain,
finding new biomarkers for faster, less invasive and more cost-efficient diagnosis,
improved drug treatment research and pathogenesis understanding is crucial. Current 
proteomics AD research is focused on finding biomarkers in alternative biological
samples, such as cerebrospinal fluid, urine and blood.

CSF is a common biofluid for AD biomarker investigations due to its proximity to
the pathology. Samples can be obtained from either the ventricular region, which is
near the brain, or the lumbar area. Mass spectrometry can then process the samples
to get the relative protein and peptide abundance. The resulting peptide and protein
abundance may differ between these samples, even when processed simultaneously.
Due to the invasive nature of ventriculostomy, access to ventricular CSF from living
beings is rare, especially those with a pathological diagnosis. Therefore, the difference
in AD biomarkers between CSF obtained via lumbar puncture and ventriculostomy
remains unclear in current literature.

## Problem

The following research questions are investigated in this thesis:

1. This project conducts an exploratory analysis of proteomic abundances along the
progression of Alzheimer’s disease from lumbar and ventricular CSF. Specifically,
by investigating the characteristics and missingness in subgroups of the data, we
will impute missing values, evaluate imputation strategies and reduce potential
bias derived from batch effects. Further, we evaluate resampling and reweighing
methods to handle the class imbalances. This exploratory analysis is done
in order to improve the performance of the data on classification tasks and
biomarker discovery and also to gain a deeper understanding of the data.

3. Predict patient’s pathological status using ML models, investigate biomarkers
on a proteomic level using feature selection methods, and identify differences
and similarities within the following subgroups:

(a) Proteins found in ventricular and lumbar CSF samples

(b) Peptides found in ventricular and lumbar CSF samples

