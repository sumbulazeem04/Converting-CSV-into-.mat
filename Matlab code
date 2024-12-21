# Converting-CSV-into-.mat
This repository contains code to convert csv files into .mat files
% Load the CSV file with 'VariableNamingRule' set to 'preserve'
csvFilePath = 'enter your own path here from computer folder /survey lung cancer.csv'; % Keep this as the uploaded file path
data = readtable(csvFilePath, 'VariableNamingRule', 'preserve');

% Assuming the last column contains the labels
feat = table2array(data(:, 1:end-1)); % Convert feature columns to array
label = table2array(data(:, end));    % Convert label column to array

% Convert to double type
feat = double(feat);
label = double(label);

% Save as .mat file
matFilePath = 'Enter your path for folder here to save into .mat article\survey_lung_cancer.mat';
save(matFilePath, 'feat', 'label');

disp(['Data successfully saved to ', matFilePath]);
