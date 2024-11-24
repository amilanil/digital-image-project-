python multi_code_inversion.py --gan_model pggan_bedroom --target_images ./examples/gan_inversion/bedroom --outputs ./gan_inversion_bedroom --composing_layer 6 --z_number 20

python colorization.py --gan_model pggan_bedroom --target_images ./examples/colorization/bedroom --outputs ./colorization --composing_layer 6 --z_number 20 

python inpainting.py --gan_model pggan_churchoutdoor --target_images ./examples/inpainting/church --outputs ./inpainting --mask ./examples/masks/mask-1.png --composing_layer 4 --z_number 30

python face_semantic_editing.py --gan_model pggan_celebahq --target_images ./examples/face --outputs ./face_manipulation --attribute_name age --composing_layer 6 --z_number 30

python super_resolution.py --gan_model pggan_celebahq --target_images ./examples/superresolution --outputs ./SR_face --factor 16 --composing_layer 6 --z_number 20
