# Project-Pixel
this is my code for my first game pixel
extends Node2D


# Called when the node enters the scene tree for the first time.
func _ready() -> void:
	
	pass # Replace with function body.

func _physics_process(delta: float) -> void:
	if ( Input.is_action_pressed("ui_right")) :
		$CharacterBody2D.move_and_collide(Vector2(10,0))
	if ( Input.is_action_pressed("ui_left")) :
		$CharacterBody2D.move_and_collide(Vector2(-10,0))
	if ( Input.is_action_pressed("ui_up")) :
		$CharacterBody2D.move_and_collide(Vector2(0,-10))
	if ( Input.is_action_pressed("ui_down")) :
		$CharacterBody2D.move_and_collide(Vector2(0,10))
	pass
	
# Called every frame. 'delta' is the elapsed time since the previous frame.

func _process(delta: float) -> void:
	#if ( Input.is_action_pressed("ui_right")) :
		#$karakter.position = $karakter.position + Vector2(10,0) 
	#if ( Input.is_action_pressed("ui_left")) :
		#$karakter.position = $karakter.position + Vector2(-10,0) 
	#if ( Input.is_action_pressed("ui_up")) :
		#$karakter.position = $karakter.position + Vector2(0,-10) 
	#if ( Input.is_action_pressed("ui_down")) :
		#$karakter.position = $karakter.position + Vector2(0,10) 
		#
	pass
