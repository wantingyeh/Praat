# Praat

## create-textgrid-forall-DIME
1. Create textgrids for all wav files in the same directory.
2. Automatically detect the space and the sounding part
3. Generate 3 tiers: (1) parent's ID, (2)Infant's ID, and (3) silence and sounding parts

## Noise deduction
1. Use spectral substraction method to denoise the ambient noise
2. Parameters: window length 0.025 s, filter frequency range: 50 - 120000
3. Smoothing: 40 Hz
4. Reference for the used parameters: S.F. Boll (1979): "Suppression of acoustic noise in speech using spectral subtraction."IEEE Transactions on ASSP 27: 113–120.

## Intensity
1. Scales the intensity of all the files in the same directory

## save_intervals_to_wav_sound_files_text
1. This script saves each interval in the selected IntervalTier of a TextGrid to a separate WAV sound file.
2. The source sound must be a LongSound object, and both the TextGrid and the LongSound must have identical names and they have to be selected before running the script.
3. Files are named with running index numbers.
4. A text file is created from the interval labels. Each line in the text file refers to a sound file 
5. This script is distributed under the GNU General Public License. (by 8.3.2002 Mietta Lennes)

## save-to-PitchFile-PitchInfo
1. automatically save .Pitch and .PitchTier from a folder (only search for wav files) 
2. extract frequency info: F0min, F0max, F0mean, F0std, slope, in Hertz and semitones

## BatchConvertTxt.xlsm
1. A vba script from excel
2. Convert all the textgrids to txt files in one directory, so that we can use the txt files to put in excel file for further coding
